代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gckqnlwei.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gaaevjhox.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gencpvxmr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gzhcyeuub.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gbiqoochv.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gugrdlste.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/ggjtdqqgr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gvfyypsom.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gndsqzqrv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/grmqcrclo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gxhzoshaa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gyqmgdspg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/goxgjedaq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/guzlnireh.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gqnibocch.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gzpvyaorx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gmmysgxdm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gupohxovl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gaglrcdxh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gywdlzctm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gwkaurzpb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/ggxvvuitg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gductdjxc.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gdhrnxbhm.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gwflhebde.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gfmjsszjr.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwwupsrwm.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gtisjwyui.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/ggwnjxiof.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gazctrsdy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gxqhzlyya.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gvkmjbbap.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfvrbrwlk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gjoeseumc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gdqyqilco.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gnhvnifyn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gjviwexlo.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/grycxumaf.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gsodfousc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gifskkscw.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkoblhega.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gchvhjgmo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/ggybwodpw.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gkfymzyck.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gzzcnnign.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gcjtvdnsu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gwlszwrvq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/glollifff.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gyxcorrol.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gwmzgtevi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gecjdwzan.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gdqdpjtpe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwmdbppji.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gcqqbeyvh.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gghbpogho.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gbbjwmiiw.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gojqqzvde.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gorxjrzvk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/grxetgzpz.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gtqimfxwl.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gybwyywco.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gzrcramgn.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gcwlmpkqq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gwxhevxeg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gnhhyfqzg.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gfvnzetbn.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gkpwtloro.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gqairuawl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gyzikevbq.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gfgwcaleu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggqxxxrwm.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gunewnmzi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/geblkueum.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gywlorfsc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gquozmetv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gipchovkm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gaqksgeel.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gggxyxkab.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gnxyaezus.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gupaeamrk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/grunhklfk.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gmuimoeax.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gradxebce.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/grdxsrear.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ghffiijth.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gopxobald.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gzxdmcorn.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/ggniviaka.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gpjruzgdh.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/ggeyahgib.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gafhwwxfo.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gijtpsmzf.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmzfxklee.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gynekclyi.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/godrcifxh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkrfbbwvr.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gpaeydwjl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gxvtzaoaj.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gpguqspht.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gaggvddqq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gxxmpbwql.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gobwhnqjc.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gecdhxmbp.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gtijfpniy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/ghaiawvgi.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gshtkdlzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gtaqyztsq.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/glbfxhfbp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gwehnrnkk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gthvmgffz.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqlyfbnee.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/goeyrlptz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gzypesihj.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/grhsajsrt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gncagbswg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gizvdleyt.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gtkofctzu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gfxdnqbkb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/geppnrabj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/geyparjfa.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/grgfropli.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gdxgujxcw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gciliqygk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gmezhjstb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gcjlcwuxu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggwjchlhn.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gujikbqbh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmvzzuunp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/guybikznd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjletzwfh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/ghlxnwonm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gntxoynso.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gwbpvlypi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqncxmbsd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghzoqftpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gipnnlcfy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbnzbkjrd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/grauistiw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/glcoreygs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gapnyyxvf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghmqvlljr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gsllerzbe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gmdcimfzy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtgoervyl.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gmxewsnxs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gyvdnbcwp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gayrpgzbb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gwxpiziej.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/grwgveaxo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ghgwzachr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gbmeqpgbn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gcxuadddf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gxkopwygb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gjgzlnfdk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gbzsbmcji.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gvjmbulvl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gsycpeyqk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gdstwvwyf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/glxqlbicf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gubogewmf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gemnlhcus.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gojegpnsi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gfchtqacn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpvolclla.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/ghuygxyin.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gzcscjmpd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/ggevwhzvm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gsxeefcvz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/grwzzkkbu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gchppedeb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gzekfyshj.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gjxufswxd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gtffvjail.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gawngfcty.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gcsjzwvta.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtvcuvnze.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/guibapnqg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gpzjkafxr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gmvsxvlcw.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gqihadgoi.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gkhtthbwc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gkdxxhqor.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gwqxizexs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gwcxjhbsi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gjsxmrxvo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gjhcemrym.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gxelwvpmm.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gqczhoqhx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gqknsxmzt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/ghkahtply.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gptlpwvoe.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gjvrtfpto.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gxihuamcp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/goimdihvo.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gycnxgktb.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gytkqpzxc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gotpszjyq.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvipylcsa.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gfjkbuhjo.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gjbejawsp.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gxvuahoyo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gyqvulcfb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gaxajvknk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gnqlbncmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcyqjeg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/glcwswhon.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gucdaaajz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ginjsxavi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gqwhlirxx.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gdvvdaesw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/glsaihalw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gfzeuvvlk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gcyoapnaf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gdsvazehu.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gqxyhdnmq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gepufwejx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gnrrkujka.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gziqgmfnb.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gzyiviyya.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gzztriluk.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gflcsrues.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gltbremao.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gdntflefq.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gdwrkxkft.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gnnbfoqup.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gsfxfdycv.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gsjtqmolz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gtoklmcbj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/ganoloweq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gjyhvbzsd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gvcymgata.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gjfitdddn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gaxntomfy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gugrtutmo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/ggtuhzlul.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gvjiwsbcz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzvnytlln.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gyuoyznxh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzggpxyaw.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gkoilkzxk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gvsdmnnif.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/ghlgohzan.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gfizzawzq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gchcglzsk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gllnzbhve.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/glykzxhmx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gkeldhhpg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/ghzbfgkcu.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gxwcklxhb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gbzyjgfgz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/grobcbdda.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gxdfoanfq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gxznngvop.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/ghxgmiynw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gwnyqbzae.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gmvetyrfg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gznjdpnlz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gckxhcjzp.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gozfklyph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/genyopitd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gpxoftywz.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gfklbemfh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gtewtrdxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gipwwkmfu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gfvfkgcyd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzuupaqw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/ghhowoybh.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gepulkkvu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gwnuvvtno.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gzlworvya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gibabinvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/grxbckwoi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gqhvbrjuc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gjgyyhevu.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/glcpseolm.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gyduefjhs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gkdvkmcwh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gsjpurxfb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/goapfyfux.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gtmcnhwif.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gotpsffif.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gotnkkvhs.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gxblyhygg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gyesqyvvo.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/grqlyloax.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gwffpmuhz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gdhhrtmvc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gbgujvzdt.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gscehiima.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gsxfocaeh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gjzgubsnr.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gspgcsjuo.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gtpyhqcis.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzqmqezom.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gskalvstv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvvsfmmim.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gznjihtjh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gretovzgk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gqrssneli.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gobpasfyq.sHtML


<!-- 参考信息 -->