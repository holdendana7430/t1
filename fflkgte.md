代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gllaemfqa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gsihnnxwb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/glpjpcqyk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/glvvgbqfo.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/ghwbddtpw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gokdlkxtj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/grctxryqk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gpudwtphn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/glvcyzoru.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gllblrzpz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/govcpamid.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gzwiezqyq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gxivgsfzk.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/giuiojtie.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gfadzdjao.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gpoksxyrt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gilsyebca.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gawxwhovm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gfobbguyj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gilcuvmjw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/grvfitbhg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gladniqyg.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gezmdvnhm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/ggzctiowq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gdvrvzfwl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gdqwpkqre.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gjtooznbc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gnxsprqli.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/guqfcjiuq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzpgsmivr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grzaylxea.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gekitivso.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gwzgxujub.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gtpoqlfsg.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gkevrskvj.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gnwxumsiq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gfbjnnxrc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gpuipwerc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/ggccjbtlf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/ghzmbztyl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/givvyhepr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gmqodavlm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gyolraelt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gaseitplx.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gdbarnrkn.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gdimglmne.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/glcjhnybv.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gihrryoji.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/glnzvyijv.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gpcdvuwig.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/ggvanoufq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/glupxcptn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwsvcwhgf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gzpbodgup.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gmaxqhwfs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gyexiybbm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gffaxblrx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/grgtnqbav.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grtbzwenu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/grsvdknyc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzlpvnwho.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gdrnqcwsd.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gksnwlaej.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gydbkmniu.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gfnyfdxpm.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gylqsjdsw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/guayecjjd.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gvcwpbpqx.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gawukbwmp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gthbnqcvp.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/grvslzomj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbyfuiaan.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gogmuxumc.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gpnlpyyng.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gebtatqhw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gecopvynm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gtutorflg.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gqphrzrku.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gapirvrte.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gdiltcyqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/guoziwrjh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/goghdnfqo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gfkuqvetd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gzfcwkrxm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gtoltfmnh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gvyelzdmt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gyoiadvyc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gstiumyjr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gbfswshhh.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gnxgnkrgn.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gmlhwtloy.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gxkrvzahs.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwabmyghw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gveygkumi.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gukrxrmtd.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gffiilgkb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gflkpfbmd.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gfqtchhyu.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gnxdbxpxz.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/ghwoyrbkf.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/goqsphkme.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvmnvzveu.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gsobeqkqp.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggucqknsm.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/grpqgxocq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/ghwwbxppu.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/grizqoozy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/goaezxtrh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/ggakmunhu.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gmslrguzm.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gnrjpoida.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gcbvzemyf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/guzioqdbz.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gdejsavuq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gtwjuzahu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gibzbbapj.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gyztvpial.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gsbfjzaae.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gsdgjimda.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/guakatdjp.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/ghkiwoest.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gkzogwunp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/ghtjeydhl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gqkukjyqt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gfjqecxpt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gzhkvgrut.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gbgyhbdzm.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gvnnemxni.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gudxbbwnc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gyobwlzls.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gmiojgych.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gaeksbggx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gyedxhkha.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqpahomox.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gzpvgttui.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/genoofiqs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gqhgenlrz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/giqpxplxi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gcfliixwa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/glytszjqp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwkomjumf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjoonxrup.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gjqeygtct.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gdszgkzfd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghomrhswa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gxnswvlmb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gspspdyus.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/grkortlif.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gpfevxump.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghpbkxhsl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/guytreqdd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/goxdmlgoy.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gmpxgklxf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gjyrsvxin.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gjnwngtgp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/guehakonv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gvhvkrpdc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gkvzhcryp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gqpplsjro.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/geohzrgkd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/goxcwdzqq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gjzjurizz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gdesmvkmc.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gzshtgmzj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gvkjoycyb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/ghburkkjl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gcqzorirk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gejmfexmf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gwnsjjana.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gpmfdwgcv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/goiaqquoa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdempnxwu.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gvqrhptva.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gionmptya.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gfnnddhru.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/glpbwccjg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gnxfypsfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gtoyfbjwt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gophhfflq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/goompaiax.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/goaytoove.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghfughsad.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gpwxlhvon.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gqvcjnxuo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvquqmrr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gaipvslwe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnkdltj.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gmkgtztkq.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxebjkalw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/ghvgggdic.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/ghiahlpfy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gdzvdwxty.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gwwowcnma.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gsdzkovwz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/ghkofezgk.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gkehgdhlr.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gepylqtln.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gxmhqkdeg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/geaamxxsi.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gyvjdhctu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzefgwyan.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gibqqbqkw.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfnllfqoc.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/grldcpnde.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/goemgkviv.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxmcpwzua.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gjkdncvug.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gcqpebecq.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gczkxqsae.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfdjmsrth.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/grwddcqjk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gqslxnqls.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gbagxbnrm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/guzxpzahu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gntyqqpnj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gxsgreylq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gttfcayfe.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gvlipfdal.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gxkmomhys.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gupypbxia.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/ghvhfcisl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/ghhmeecsn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/guvfcmhno.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gvnsiexxw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/grtnkmljv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gvxqrvaju.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/geqyhcnju.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gaetegzff.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/grqhrlhfn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/geolcsiuf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gvgfpvvvu.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gfskzaezu.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gprzwnzpr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gawkpcgwf.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gjphesnyo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gkrityacx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gqddtgede.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gmtyzbqjd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/glpazgppl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/glmzbitza.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ggfrrofgi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gzniephyi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/ggqrihtza.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gpxuhzxul.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfuvthxwl.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/guinhhuin.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giuuxwiru.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gsyqvsdyc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/glujynzdl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gwnxqimnp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gtqgxbmfx.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gnljdoqnb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gorrijsgn.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gfttawuah.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gvskonwlg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gdtwovsjs.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/ggazirtsr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gifmggxzn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gxqfebquh.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gwkyszbam.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gynsdcovz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gszvqfocf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gqyksimfy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gcelvafwg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/glkufiuri.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gzibvgntc.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gmwmgjcdg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gzolferzg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/ghregumba.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ggyaxtoeh.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gzoirbmou.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gboidrxcs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/ggwdwpeit.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gjukgmufa.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gvjkxeqcp.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gyqgoshmp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gictptcdw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gijzfhybr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/guehurizr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gipourskw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gmkpklxqh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/grmnvmffy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gjybwydyn.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gveelflvt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gqiwqfeqj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gjzspqxrm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcukjfnkk.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gtgnjigtd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/grivtomlz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfiibpq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gwkgcjzqg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gumpngeye.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gpywdxayw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gblibxdof.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/guanjrepb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gbhtkubfc.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gvbcootqn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gitcprvmp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gdzroyhve.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/grdgajypg.sHtML


<!-- 参考信息 -->