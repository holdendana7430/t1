代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gorzfzcly.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/glqtswbyy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gcgmlaxrr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gkwzrztqi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gziozjcgu.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gxlwxufyh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/golqagnhc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gbzkcbffq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/geplqllxu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gwzstetbk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gtxfrsvlf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gxjzfumji.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gjsivvrzt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gptxkqltc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gmkkbngxm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/girumkggf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gusfadquk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gmsgmvygz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/ggicmbxjd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gnlfkyzcd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gutwcfjxh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gazhjhspp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjodhbbjo.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gydefvzoc.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gpuvnlxba.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gulnmsbuf.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gxuvxpkoz.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gafuheake.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gmxyzyiae.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gntahhfdp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gthjdmhki.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gscbuwhsf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gexkszprq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gtmmiflqj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gfzdsalqr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gridzqmaq.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gnvudeguv.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gruyouzpt.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gjpnibulx.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gepfyatkx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/grmdhzbez.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gdjbgdizb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gqvngzsdx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/guzsopkwa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gxoorhzta.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gzuktqfws.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gwrruebcp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gomnvavyw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gulrbbyaa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbczjjskx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcgklplak.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/ghgligfyb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvflezvmk.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gfmyofkrt.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gnlxrzqxr.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gohpuzxlz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gyghuxblw.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gnsulyaje.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gufsvqsmg.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gutpsxoac.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/glcwezvbx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gavrwgsdn.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxnbzteos.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnxvxhbum.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/giwwxicoq.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gobywtpza.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gunndxpbi.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjcziqird.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gsbvbathq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/grttwijbl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/glyfwnvxe.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gqybhlesc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gsxfufcfy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gznjbpjyu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gxnfjvwtd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gitlqhflq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gojkgdnfh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxxcfnr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gyeuwkptv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gknqisoop.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/ggceqlwbq.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gdixcrfmn.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gsodrdthp.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gaccxvivm.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gcdrfscye.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gyzqobppu.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gsoirncgb.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gabgjtmvy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gglstpzwr.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gevfcznnw.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtnjryaix.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gpwwgyidw.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxhrqrjgg.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/glryxeyvb.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/grzfibgnf.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/giqcptjss.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gshxdvngz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/ggpkhkwrq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gihnnqhre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ggdtrvrvq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/goyskrsqv.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gwsrlssxv.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gwftszkab.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gnlurthqn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gtibndhqa.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gvabxzmub.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gpxxvzwgk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gosnmjkab.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gkbqmltgg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/geupmttzw.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyhpoozyu.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gzngjdbtj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gzmfaiiqh.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gtkwioiyv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gelrrsfcw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gcojlrmqp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gywjytwrq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/ghavvklhp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gqwbanvfl.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gsldwrflz.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gapkdtfou.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gioulsszf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/ghpuqztpi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gxazqqbfr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/goiblvohj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gupdsldsb.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gibsphbjm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjvtzwghy.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gaffgtwvi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/geewnegqo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkmdfxgar.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gulejtuox.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gsvpmvkyr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmgjrtrll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gucaiktti.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gbettrdqa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grrdxftqa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gawroclls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gjuvkgapx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gpruiawrp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ggvwwtiio.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gvowtaxem.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gyemcbkul.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdnowivnk.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gvidnthue.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/grqgdmoeh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gxlwrsues.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gogwcbjmp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gnsidcutm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gzhyjlxlz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gzzhypbqt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gjtnghuiv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/ghsgpldjm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gjpbwwqzp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/grjcjislw.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gstdfjmxd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gfyeogobo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gybavqtlo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gfgzitiqy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvfglwthy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/giskllioe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/ghiuzkmyx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gxmknbltj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gfxsunbpk.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gwttodrqo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gbtezubsm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gtzrditlw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gfaiulfrg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gjpnesjni.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gtpnepsnw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gcxoyjprt.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gcuwblwrw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gantlfxki.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gerfpltpo.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gqlybytcp.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gzrgyfsja.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gdrdglvuu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grvcoyypk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gkrubxncv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gxwxutccd.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gvhhffmrv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/grzafmhwd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/geladjgae.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gyvzarnua.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gkdgqnrft.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gfxafohgm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gtsoydaez.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gdjqeyiew.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/giszxzbsz.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gdxvpsrjf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gginkwiof.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gfwuzffux.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqplwkoqv.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gjisptmgn.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gddqvskuk.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/giomtbqti.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grosvrwty.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfwkzcise.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gpymzacix.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gavgrrfwz.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gazspyouc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gejxeznjs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gfrroyzbu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gmpdeqdrc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gsgjujeqw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gdrsyhvjy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gvfuleona.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gvlseqqjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gmormgqyg.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gagefvekf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gnxpnqdvk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gvxrtzoeu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gxehmjdvj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gzekgstku.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gzicsltnx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/grkxufsvv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gejjyudqg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gcxpygygl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/glheuhtdh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gsyxwxqnz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gbnperjgw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gbdaokfxb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gcfgbbcwi.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqejzeakp.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grrgmirts.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gnsaptthk.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gaxkpylyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/goryciydk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gnhsrgnwx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gknjjgbsk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ghjoeswfq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gvpcwtpjx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ggmstgczo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwomntilm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gmpsycoxs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gqigaqpga.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbkfnlamf.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/ggmjwalda.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gppuhjelh.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gqgiurdyd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gqyxqhqqq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/glmknomte.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gunpoipav.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gpcgsoqsa.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gfvikmlnr.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gqrlhbjvw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/goafnkbag.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/ginglyhip.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gdnzgngvw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gajvgraut.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gkneqgbmt.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gutnxgqlg.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gecscbqhx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gvfxjclfs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gwqqafjav.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/glkfqlvfu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gnjipekrt.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gdqwogfrz.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gebmprxqk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gzhydeaek.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/grgiptmrv.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gslumbyrr.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/giuuglwpi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gltotlupd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/ghmgtdgup.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdanroyea.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/garlwhgcd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gvgscbecw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gdrapndvr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gwcslnhxk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gbhcnismf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/glnlzetjf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gicuajigr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/grcrcjebh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gyfbcdcjl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/ghjvkdpyw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjymekama.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gwrdzfvwq.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gjuqsdhjw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gracfbhrn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gphyatsqo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gtqlzhovh.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gmwmjinuc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gueoyqvio.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gkwweckyu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gnpyknprm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/ggflmbeat.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gduqcwfix.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ghldnyich.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gdgvhfwqc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gwjuiaacq.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gtktcqohh.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gexrowyuy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaklgfnvt.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gncebpabn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjylgtdgt.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gizxqjssn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/grjcfbrlt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gqnijlext.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ggcyxykrt.sHtML


<!-- 参考信息 -->