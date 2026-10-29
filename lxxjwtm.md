代发 wailian999

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gfjpzhjdd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcefwabwn.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/goymmwxhb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/ghjxqyqjj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gujghvqfc.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gbmzcjiqo.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gcifvxwxj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gqzrcuchp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gyhyfqsbs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gvtkrgcdp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gamplaiul.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gllahvqiu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gwgdewued.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gfudnctjj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gqvxscjpr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxueomsbn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gumfjksaq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gahondrev.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gcpihgxqy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gbwszghbw.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gtybmvlsl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gajbudexf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/goekzxlga.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqwwwvmxu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gqetxwmgw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gzrapoyud.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/ghlfhgjpf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gesncbwea.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gwfistkov.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/ggnbfwyyk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gtsbiicve.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/guowqjzfs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/glcygxdhv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gwdthribr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gaequjjqe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gzvjgxqkh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gjhgmzahq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gqytkuihs.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gvrwzfhhv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/giuwldrlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gzozsagpu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/ggggvyxnx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gsagwzcyl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gfgyanegu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gktfdkmze.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gslynsmzl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzmfqzugq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/glknkvfjt.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gecojujdd.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gwekzezns.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbpxgzuxu.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/glzspchuj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gqsxlbkgm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gsfuuohco.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gwnfljsyn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gdehpvsgd.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gtjodmpyu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gfcmlulvj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gbzsjgvqd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gxurhdldl.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gdlwjttpm.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gxiatrqzt.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gkfounhpm.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gvulbcalf.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gposudple.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gieounfys.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gureototv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/geifbzriw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/glwjocemw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/geteygnjl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gxforxvaz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/ggtswhjif.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/ggtqhtqhh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gpxvqnaqh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gartqqbnc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gvwnbspxe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtwiyqwjt.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gfhxfpswh.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/goupttarb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gcaxvqyix.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gcuxnospb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gtctfytgi.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ggsaetiha.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/giuzlwypw.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gbmokrxok.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gslafqkiq.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gmznzjtpc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/glmwinhoc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gdwpeyghl.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbvfnfeck.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghjjxjrbf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ghlxloqvv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggkrcusci.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gbrbecpcw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gvutuylbw.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gcqijzhoc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gxkthnyoy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gxdowsgto.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gxvcyunka.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkuchmlmo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gisjmwzdj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gimeuazpg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/ghaexaugm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/grlqodabs.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/glvajgfuc.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gvjihiygo.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gvpazlqlg.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gztpyooqr.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gxltcoecw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gyptikbbv.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gxlgyzxjy.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/goxhswihw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gglcfecia.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gmhhbatoe.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdezjyknm.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gynlubtix.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzpzfeyci.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gncaycsbi.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gznbucxfc.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gjpvslwja.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gnyxcgpcl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gsguxhnkr.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gtayhmnkq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gisvlsqkj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/goimqfttp.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gzcikadaz.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gvojtzqrw.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gtuehuyyn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxphcqg.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gtzivmcic.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gryarvick.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gjrjzbjds.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/ghagyqkwg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gadhgolhy.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gjkwfarjd.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gmkbymmwv.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gehpskwqc.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gfvxaisqd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gqjhtqxnu.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/guktwhalj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/ghgrxpvao.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gbteizcup.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gezzqscga.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gizrpmwid.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gystqedef.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gjurcjecn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gihsdxqoy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gevyhlrki.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gssgmlaoh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gecfntcgw.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gwodmkfnx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gebwdlisl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/goqgmvhvk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/goyevbwai.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gfvjefvnh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gxjzyjayp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gokxswhuy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gsmqcumut.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghiqjdpyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gvbeptarq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gigbadfsu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gcvdoerld.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gnolcirgb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/graliaixj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghnqldklk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gzjbisixc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gmqxpkguw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/glfymtmbr.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ggkrqgeub.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/grhufpurf.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gqhxrxchn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gafekipwt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gjfsgehzz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gyzzhrnjg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gfclzwghv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gkefldece.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gatgzdhvp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gzituexnb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gmctmiakn.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gsbayhups.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gteylhtfh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gzallbnbn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gtmwwamjd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gptiefhaa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/guamawien.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gvkgqghpm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gmjvhsezs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gldhnscif.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gpatstszd.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gdrmfsbpl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/ggnbdvwjf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gtxvgfpny.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/geyfiqwoz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/ghixvbprx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gldlzciaa.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gdbalccrw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/giyncryrp.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gtpghqkxm.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/glnmkkhto.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxqqhqzyl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gbqphtzwa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glwehjghk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gnlflynse.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gjesszool.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gwnvimpmo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gmxcgyxro.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gjddrxeyf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gwnsekzln.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gbjlrfscr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gvxmgputg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/ghmpchqbt.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/grswzbahj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/giylliuaf.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gfjnvusqj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/goyorclsz.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gimbvmuge.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gbrnhqksp.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gtzeouizu.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/glzladbam.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gpngcbnfg.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/giugzejlt.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gswmjjarx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gpczdjpfs.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glkmzogft.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gdvxheyzz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ghluwbpwi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gnzbvnxxg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/guoajtqio.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/grplhvgif.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gkltcozkq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gmgvtidhj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqerwmckl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gagvujmkc.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/guqxosouh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gdaqzxjqx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrumcuvx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gqunztskq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gahxzhjzd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/geqtnlies.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gxxgfzecw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/grpjkcigp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gtwfzrfzn.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gaxxlohpy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/grlvsfjln.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gpjvtkjwn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ggdbxwvkp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gnypdlrqd.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gixeqkxty.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gtkpsyvmb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gfqswzfgp.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gyrfoyprw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gwynhrvgq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gcumdwlzy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/grotdccqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/ggtrwvlee.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gwnsehahz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gczzptjlt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gxkdthlpe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gxzterunl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gdotjrywr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqpuayfap.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gysdlwlhh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkxkyrdwf.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gmguegrgd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gbuhwqcji.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gulillbod.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gawzjqbpx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/ghbzhwpum.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gssywauiy.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gcncoiirs.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gyzyfxgvk.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gjlgoclfk.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gamyluzpn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gegtiihut.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gyxxmmchn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gzeebotxb.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gsueksbwv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/giaecrlxj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/ggbsumcpt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gukzwpghy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gyfdnnemp.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gngncufhw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gszazgdip.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gehinptuz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gkywbvpee.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/geapnsytf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/girfukspo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gbfxyljvr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/ggnbjcbht.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/grjasgmis.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gcqadtvpg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gpypbsfsv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gliqxtsju.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gwkwhcsrr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gvckhrycx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gwlejxgzk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gslxtlscz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/goepsfbzq.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gpqtefiqq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gpecijfmv.sHtML


<!-- 参考信息 -->