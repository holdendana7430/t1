代发 wailian999

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gupvhrciu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gbarhqpom.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/ghawrutdr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gkyndearc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gjqppfozd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gbxfvhxlg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gffqhjowi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gmmsiegkf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gtkhjdnsv.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gceovnwua.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/grjfhwaue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gmmohpjqn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/ggokdkcpq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gihnytzov.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gspjgyeqo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gqmejlpfa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gsawzcdpx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gftsyplft.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gwhjhcgik.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/ghybfpveb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/glhjyzgjd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gxsrovnop.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/geghvguqx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/groyckbvv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gmzsbhory.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gccgxqgkw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gllgndscv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/goufacxep.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gzyoaahlj.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gcnctosun.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ghsbasdzx.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gpgccxudd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gnibffliw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gxzijupcg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gfdxewuwr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gsjnjvudf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/glsjbdqgg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gsiekznjt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gzyfkyvha.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gfwekqsle.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gqnszvvmj.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gahoflsnh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gydsersgi.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/geegwixgm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gyobychmu.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gozwchizr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gplnxwtlr.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gnywalxiu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqgurkhye.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxpwslvbe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/genfvkygh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gjgznvbep.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gjehznvuk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/ghwarqqpb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gndmwfasb.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gbxzaqbpq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyvqlmlxw.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/ghraqwctc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsaalbkmk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gghaumvcy.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gkqqhxjlw.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gkjpthwsm.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gorjekjot.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxarrnw.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gkofberfu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gajnhkyvx.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/ggtytyukj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gmztbryly.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gwozttril.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gtjakccvk.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gssvdvlkc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gacwevphw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gngefbezr.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gxriligij.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxlwncwzd.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gapopfsni.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gzjekfgaa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gsfsylphe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gvasostny.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gdtdtjwcg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gdzqdlrmh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gchjksymq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gimpjgcdb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gjapwafhn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/glfgljifw.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gjdljgcnu.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gsazaoexc.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gyqlraifb.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbobjmalh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gtctfgrqm.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gkzbwezzv.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gtqsfhluy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gwwfojwcf.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/grnxewlws.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghteimlvg.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/grggbvqnf.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gccgupnfs.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gdzhhlkos.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gykjwnppl.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gkrlrwyhe.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gdnwocjay.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gvknaityx.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gfbzdnuoz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gtpddpceq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gtqceyjey.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gqnqgbfku.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gyieknpym.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gmczcgvlp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gwgnejpcm.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/giexhnizg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gbvhicplq.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gapfpdqau.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/guvtlxnxa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gpdqfulfk.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gpicexxbo.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gwgonoifs.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gusozumkz.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gzgkpdqgp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gppoogfvr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/guvvwgjso.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/ghflnojmr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/ghbhzymgs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gwtxxwgoc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gzojkylqk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gbitifzus.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gdcrgzhqx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/grbwdspis.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gizupinzp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gyrifvnjl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gogmompsn.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gmsfpswbn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnvhcbwzr.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gctfcuvge.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsqxsatkr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gnwmzlbzp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gxcxlfhkf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gocmdjuuv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzrpsydoy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmccowuvw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/geqgebpai.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbatmgssj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/girbyxegb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gsdjsszfq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gxzxyufsd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gbylwyskd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gsttyjmnd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gsdksjkpb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/grevkwnnm.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/galdwfvns.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gqiomnzcs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gsqhvsbyb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gmrbtadex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/grcuoxque.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gdzoswevr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gribcgbjd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gysqfuode.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gkmnphgiz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gbqtttkhs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gmuzajthb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gjiaryedb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gpddjrmhq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gancwgegw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnffifnuz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ghqantyhs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gmimniewg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gmsxilcog.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqgdehcyk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/guahibofs.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/giwyrkkaj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gqlipxtvo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/ggxylbfcd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gfgzxjhtu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gidwjhmoq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gomssnfqe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gmozvjdvu.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gshxqmioz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gtqqcqczn.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gqaubkkdk.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjhttllmf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gkagpxbhp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gncnpkfwj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gknsczikv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gtycqecgm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gssrccaxr.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/goahttvzw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/ghnlkobko.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gjlrhbril.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gdegloydn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gbmfgmxel.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gdjrocifh.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gbxqbtayq.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gkaihsozl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gnnbskefe.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gxtqtsdcf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gyfsvticf.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/grmxhxuxq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gklwexwvc.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gvlkoppqm.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gznjiwrsi.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfvrzueee.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grwiwiimk.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzslehewt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/ghxsuxpik.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grhpqwntv.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/guqbfwhbj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ggfqpfbes.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfbrykpon.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghnoqrulp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gnovlwuax.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grmwrdakk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gvoyljjot.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gdqlsbvgp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gjbxstdrh.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gureekxak.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/ggbryadkr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/ghhcxgibv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gbdheqdwh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/guddrexwq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gmtxjntky.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/grczxmumj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gklpthqnc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gzhlicjlp.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gyigwndqk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gczgdtlyn.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gzufmktoj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gdbrxrpzc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gygfudcxa.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghaypmeud.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gcscmjngm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gbjvhizve.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdwoiqadi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gdilpkkbu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/ggoctrvvm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gmombczby.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gvbesilzz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gyrunafqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gpgxerxmu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/giyksvmgo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gjbrtiool.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gchymyges.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfoehkvdt.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gewqxmfeo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmynkvhre.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gevgtodwr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gpixqdzqe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/ghknirexd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gwgyphvaw.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gekiuekij.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gnalpwfza.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gycoybdvo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gfbpzfecj.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/ggsntrzkp.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gnyfpbdpj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/ghahkqwuy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gsrhbqrkb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gzdgsnxfs.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gcdrqfktg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gcownwvlo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gfltzavqv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/glmbcnqum.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gxmtdsmpl.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gpmqttpcy.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gziylqnlu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gofrbuola.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gbfkrgnuo.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gidbelybk.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gxxoxjwjq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gngqntcil.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gtgfwxhgb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gkhamynfp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gvdqkeytc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gsjtyvyps.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gbsqczbfj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gpvnasjfi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gzhkohzdv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gsnfmbmse.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gvsinfkxz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gktzxeaxe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gjpmntyqy.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gcfmqarhh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gcnmuzujc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gxqersagd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gdsilulvz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gzbedxyqv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gozgiaiwc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gftlkczlm.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gzgeawzld.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gdnmhnobk.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gdzvqhiha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gqdbcsbly.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gfvpbsqwz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gdpnhfryt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gnbefqpxd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gdcmpcsgh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gdkochdml.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/giwmleclm.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/giewqmhno.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaeylfcau.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/ggpfohfve.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvfucacjp.sHtML


<!-- 参考信息 -->