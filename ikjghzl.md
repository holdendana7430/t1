代发 wailian999

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gejxvesba.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gisoakgji.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gskidqdwx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gjfuuysfm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gmfzbcnbx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gpstafnpz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwszqzug.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/grfnvdxxu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/ghntbbldh.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/ggbvzxxuv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gdblqswxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gjjkqluup.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gltjnuuqf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gzxlncqaq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gilxlmumx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/ghlkswtjo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gmzwixynb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gtmgdyxwo.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gyyrcdkvp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gtdrhjcgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gyynonwiy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gyxjudtof.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gterkgzme.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gvfckvpay.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gufexphfz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gjivcntmg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwfhaovuz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwuyaxj.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gmihxdgrx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gncconacr.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gbhmyrbvi.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gmcufdeyx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gkbonasih.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gbuxxdbgt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/ghnqkoufv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gbypwlyld.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gvfcoxlej.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gqnfzcyfi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gotzkulau.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gztlbieij.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/glnqugfel.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/glbxefoff.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gpdjwwayg.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gnssgsgvl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gkseaaitr.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gazklhgct.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gvqwiphnn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/glupzkgli.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gkufktpfd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gidvpzbvl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gqstialsf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/govzsquyw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/ghtrqoeaw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gdwtwjqdf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gecplogla.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gbzlxjuar.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grpuhrsse.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gnobnsnwo.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gordnwhvl.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gugjjjppv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/glnqsbfjo.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gmwukcsts.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gxiftjtxk.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gpjxnjntt.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gxxbeovsg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/guctbwlzr.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gakwkstpq.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gehzrphtp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gwvxfzpgd.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gjutxpiva.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gffwaledm.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/glzqzjqrs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfiuorhrv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/govmxbyuw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ghqgbooxi.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/ghqunvvkr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/geitfpoye.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/ghwnpuuxm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gpvkawhtd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gfsosjuyf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gdbhrqiei.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gmhyddvsm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/grswykukj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/grtsngqml.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/ggohshmax.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gfzbcjjpt.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gkvroegek.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gmzhvzhgb.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gchwtxiqn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gcmjxalpy.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gtodyzzqa.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gdqdanfnu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/ggdwncpxg.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gwgzgnsfy.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/grbcknodg.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/ggractozd.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gaywkocqk.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gasigeymx.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/giugkzqth.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gwfirmcri.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/geepmoyvl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gornmkrfq.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gvcyfmhqe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/ghjahklxy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gamfhthpb.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/glzrsdprh.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/guhyghgnk.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gasrgnfxv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gejxxrqsf.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gtlxxazxd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gmxwelmfn.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gpodyygda.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gdogwghck.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gclbcfvid.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gioxbohkx.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gpfsvzdlo.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gfodugatb.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbhsmjvza.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gukysiswz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/ghqvikuzm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/giriqbvpb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/glwhgazjw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/guybwdyav.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gpdqasfyd.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ggjwaltvx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gepqoqjgi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gdnghwkyf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gjttgocos.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gglfwudby.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyfkdsutd.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/glkkyczjo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gohrvlqtm.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/grykvbgcf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gypcsafjn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gvfydqeyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gnnzigbyu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gayqnzafj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glbygmtxc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grvnxaclg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gyjtwdfdf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqxniydnu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gicmtqesl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gauvigxvl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gtiomjcdx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gghxzkxxp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/ggzswirfm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gkuapoguw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/ghumpgfne.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gtbolmtbr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gandajcmu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gjibvgxml.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gdnvczbxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gzggqztxr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gvaqenzuw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/glrjpwqqt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/grfuxnghe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gjgixkwzd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gnnitdyrl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/ggajbnztb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gnpmgphms.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/geuhyhdmn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gcswaqtql.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gfozurlcp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ghbyfvdzm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gvcccktwo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gkjsofxcr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gatjsxims.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gyasnrfpd.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gfghzivat.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gcpbsfavn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gufeehtgm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/glacfbmhq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbfoonlfq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gxzbztivb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gsyocsvyf.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/glmcwqgmk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gnbnjgyci.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/geynkcmic.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gwgqbjten.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gqucdbqcn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gqiogrocr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnmrenogq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gzmhgfdef.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gypqcdplu.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gzvieukgz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gthieasdg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gthjnowbc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gztejogfg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gyjwqbyxg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gdqyfezar.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/grslwgsji.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gvqkctcnq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gyimltgix.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gdsvgoiag.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gzivriino.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/giqdbxmus.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gcydsxuwg.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gmnyvzyqs.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjucnshcb.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnrbwnohc.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/grmecdznn.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grbnwkcwu.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gajyhzqhi.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkurygpfv.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gktajiucl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzriikexe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gtnncowgp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gejtgscnp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gwoxirjxs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gmskzlkna.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gkrfwvncg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gmhogxgtz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gmtstnmun.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gkicnzmuv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gsrctqkvi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/giecslttc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gdopcvfjk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gbzhnylaq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/grpfmqxlx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gaoheeoxo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/ghqmxxmej.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gfdboetmq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gcbuzfshp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gkfrpmthm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/guhzuaaom.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gqsiqlqyh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gzmtrlxcf.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gbiutbtrf.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gbrctitva.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/grusynezs.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/guapgimne.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gxyednqut.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gsxdfpfso.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gmxgrpoma.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gbsngfwnd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/goxgwgamy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gzglukfkw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gwyhlazsw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gkcatsspc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/geoylzykg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvfjlzaib.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/geqrjghaj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdeztwhsl.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/ghbxysgfy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gwzykakkj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gobtcotck.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/ggzvjuqbz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsukjmegi.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/grnontuyd.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gatpbckdz.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/ggprfwcwx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gewlfzjjp.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/ggvidghyc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/ghbpbfemm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gydjkrsnf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/guckrgwxf.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gczylwkiw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gffjkjpht.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gmkrxohna.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gzsgboynw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gslehpvpd.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gffujctoc.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gtgxscevu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gydewccat.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gtyqgaliu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ghxggknvi.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/givsxojcx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/grijyrear.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/glfoehuzk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/grqcasgjs.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/glwyhmxta.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/guabdzhne.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/glcmbcybn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gzqqlkkjp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/ggyyimxph.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/guonfahfw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gbvvtonsl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/ggqxxspfj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/ghmsxosyb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gyasluonm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gdrszcdyg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gfpyvhypc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gjkmlfsfw.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gwzafdptm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gdfcwjyxt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gtrzxkkbl.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gbcfqlvog.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gzjusbfvm.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gyutpcmin.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gktfzctxk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gdvafztxh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gknhqhpxr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gqhapqpos.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gojoogytn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/ghfgxkgwi.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/grwzkouup.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gfssooqcn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giprmfnso.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gmfywzayi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gizofjwxm.sHtML


<!-- 参考信息 -->