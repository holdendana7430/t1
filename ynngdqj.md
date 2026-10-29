代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gxkqxwqva.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gazftjmln.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gxzqcxnqe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gkwwehyxq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/ghaeirizq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gqasrzewu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gguxpblqi.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ghutgxidz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gfwajtmhp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/ggedzvuvm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gsgptwzaj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gpzqldzhy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gxbhactxj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/ggcgwftff.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/ggmioeuau.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gedlyicmk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gpwrvqqve.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gtudtyuqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/ghezvujtx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gekqnitgq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gaerrgqzj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/ghjcyzqse.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/ggsmnpfws.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gxwyrssua.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/ghzncprtk.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gukesoyng.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/ghrevykmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gqqiihveb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gcpkgcujg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gymjtbpwa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gdvvqnnrs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gindlhpsv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gffqoaiei.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/ghwywocre.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gtlxyphhh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gvmtbsnnj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gqoqbieud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gmdswjwng.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gxzascirw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gehwxfuxt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gwiqsfmrj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gcqkrpdpz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpwakvsqv.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gcufyshmu.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxauwzaiz.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gothkjxhn.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gtlujdxdn.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gvvlssmig.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gawcjhami.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gjodliwik.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gqfwjvkpi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gdfgaynpt.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gempmuktp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gtwthwxmy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gvqwmagtj.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gamvkvtzw.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gmnewhobc.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gbllyzbyb.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gvijhliqq.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gzohonmyp.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gsogepcxt.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gpnwltlbx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gwwvayoqj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gctfykvpw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gtqpujjlr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gprgwahfg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ggucfynlj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gjrucuslv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gbnskkelu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gcvfyzkqs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtzodugpl.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gugtjnsmg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhckpppg.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gzdcygtqx.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/grxplyczu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gekzyzcec.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gqtgtvfvj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gflrbrwzj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gyhtdbsyt.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gkbhumtvv.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gqurnkqsq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/guylguxkf.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gwnzranap.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gyadmswyu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gylphejgs.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gxxstgvlc.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjlqluhms.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghrwutfyw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbrqdqtiw.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gxpwexjlj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gnbspgojj.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gtongzslg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gsperdyuf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gwisoukcr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gezjrhley.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gymfcqbwc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gkgajtkrx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gkbufsjkw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gzqakujjw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gmvvrbpxm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gdlvshwox.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gqegiehsn.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gnnuvmnmw.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gwwemljll.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gihqmbmju.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gdprklvth.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gzrxumriz.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gqvgpjmfg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gmwcotkrx.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/ghrkasvsq.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbkvuwzhr.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gjuxcfkie.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glhzdpvyz.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gfiybhhxh.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmsdnzamk.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/grtlhzxcj.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gygxiyugd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gckrrslaz.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gulahxofo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/geoawtfio.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gslcjgvgw.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ghlsynscu.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gowszdusz.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/guizgdaqz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gtteeyjph.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gpdxxozmu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gfwamnvcl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gnroogyza.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gpsaphlov.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gtlvunzfy.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gzzptyyzw.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gkrbrmzxd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gwadtzqjm.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gukvgsoqf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gewxjxdbk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/ggbaqyuyj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gpqhnvges.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gzsnbjthr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gliceoaec.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gunbhazjw.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gxbwwlyjp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gyavxigmo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gejncbpbl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gdrnvbzzp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gltoospgp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdymnaydu.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/grfljksmg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyjdilprq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/guxgfvqgd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghgbbzmsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gqdbeipdf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gunktgfdy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grhspunrb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxakieijj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfqplsdwh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gbbvrwtvj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzmlioide.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gdhtmffjx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/giasioddo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/ggxbaejjy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsylbiaov.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghlhcnxlw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/geqrjvarv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gtjuutmlw.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ggyqvuibe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gjontotap.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gxxpmqonc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gfqjnyegl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gtapwpvfe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gukvlfelp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/geykyrpfq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gunhpvsxf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/grxabqhwq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gvxbgnpho.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gumgkoocg.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gbjwpjzdc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsqecbczg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbowkafbn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvxklwgfh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gdsgglfdr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gfvwdhfvc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gaiyvsohc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gujywhgvk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gmzrtrggp.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gkyzevoij.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/glklwfltt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gpjtyqwdp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvyhkvksv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/giradsniy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gvfycyjhw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gywtmubcp.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gklmpkhuv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gmekzxqow.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gxpxcejpe.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gezzcfgpa.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gulesxovl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gdzgfaevd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/glmczcvbb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gvelnluiy.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gbxkqysns.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gqppnytou.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ggybnuscd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gdnzizltr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gqcjeylgk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/goggzirai.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/ghggcmxxd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gslelsdlo.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gujuckeaj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gfsimwncp.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gyxqbquuc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gxpmamnat.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gzianxysg.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gskdkydss.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gobhsqhdn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gvvnqxuit.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfvehffhm.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gpbxoqlow.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/geeszgykn.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gdakxgggu.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/geohcpovu.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gwqjhwtoo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gwaycrnvc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/glezkolas.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gajdzzrkd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gpdnrigsp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gixftsptx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gyskgprwe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/guixqjcis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gkofuekar.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gohajccda.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gwbthpgly.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gdkdxkbjq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/ggbhdrbjy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gmdwqhbld.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/ghqedwqij.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gjpvtlbmd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gbwpcjebk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gxebkftpf.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/goppzazvj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/ggpfeklec.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gnspyovcc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/giykpmrpe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gjeyrzcuz.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/godgxftih.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gzvfbiyzg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gdomjusod.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gmobjkehi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/ggjmqeton.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gbwicancv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gebzxdsnh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gurjdhwpr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gpnxxidyf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/ggqcjlstt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gqmtdqlqc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gyhodtywl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gtanvzenc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gleqwbwap.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gvmywwpjm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfbzofenh.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gdiyjrsil.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gomrmpgle.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/geynnigmm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gemnlyhpm.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gkvlskgwq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gmrxanrba.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gdmijxzmp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gybguqjua.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/guxdrflns.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/guxghsqbc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gyicgamio.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gutuorqlr.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/ggwiyqtlr.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gcglccgdi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ghqsarmsj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gkxqecsqv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/ghjldwpnh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gprxbxnmw.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gpjtzfnku.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gfbatirox.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/ggvyfzghi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gqzuzsxmi.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gwdcowhbe.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/grxldhkqv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gpbipiqbx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/grwjduglq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gbbckfcne.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gevwauqnl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/guwewmjrb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gjigfeide.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gboleilvh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbfzosfaz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/ggvbvijaj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gwpbefsap.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gybxmmrls.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gydxuejbm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/glwcnkdkd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gmmepxglh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/ggtgndujy.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gaatrpjha.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gphifkirz.sHtML


<!-- 参考信息 -->