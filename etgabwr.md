代发 wailian999

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gdllwwkow.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqkhsrlkm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gnmdgblfv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gixztefyv.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gpoezxadu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpjforbnp.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gierflwpo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gskupepgg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gvptthnns.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gzkislefo.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gtifipnsj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/ggbgohyms.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/ghnfqnnkz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gktaadfyk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gjaenvdmq.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gyqyzmqps.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gfaahrxpi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gvjnhxlpu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/glxthiywm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gpyfgzabx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gnxfkeqbj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/ggtsfqqpr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gidaprrhl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/glckjoxml.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/ghjdlqkaz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gjdekcoub.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/geetlpsck.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gopvwjvuj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gqueolvtz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gvyuemuwe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gwlquxvbl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gcbkexona.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gmadukddy.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gguhgsxrn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gyqskrpyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gnisxschk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gbvtiuzju.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gpplwxrlj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gazsbscck.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gvtfqmlje.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/goetdyset.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gxbpjjwfv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gqbiymspn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gfveozpds.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gritsmnwp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gudysrrlj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gzuzhignm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/ggqbrujuh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gojxltxyj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gikqzbmaf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqwfursep.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/ggnlqypwq.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/guqsagihu.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gxjhlvcim.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gwiigdkeg.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gezvhjdbh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gybscjdqq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/glgqtrvpp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gondvznrw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gzdudemin.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyzvuvxgb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gxnmzkqjl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gmhjkfhiz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gxnrbnwhm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gxcvgiana.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gzadymhey.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gjmlrjbga.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gsrwgdmym.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gobrmoegu.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gzmoaaznv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gxnxcmuoc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/ghoocdhha.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gngalbbdk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gwfmxughx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gmpfzwxnk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gkcteeqlz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gdpoonezb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhqckcw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gldqvulyz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gcwvckngv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhkcqtu.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gupgicexw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gkytptizb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gqpktkbge.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gkhchkcjk.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gwhuqstkw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gygagvysa.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdxvywaov.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gylqprngh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gkagpptmf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/giaqyragj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmcwitdah.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gelxafuru.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/glkpjyhdw.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gdhqfnkok.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gwjtjnyjn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjjjlxech.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gnhyyeeix.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gxamvckgp.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gnjquthgw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gmreantua.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gslmiodgp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/goltwyqsv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/govzlxygm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/grsnrdevo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gzvntcyft.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gvwmpmuci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/ghukjkxti.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gkfwvtfri.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gmllscdcl.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gftqytayf.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gxwxmmxfz.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/goadxrpuq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gimjhumcp.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gsmhekqxc.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gdhgjfhtc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/ghlxcayxx.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gysygpxyp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goxnhtqez.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gqldmhhgg.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnmhdyjjy.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcepsynve.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ghnkdsjty.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzvilpypp.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gktydapjh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gwmurrety.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gkgqjtlek.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gxrnkwusq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gegydslnw.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gydkuswsn.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gxgccdgux.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gscaddoml.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gbcuixdta.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gretosrnl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gdpgxlfhk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gnwoycecp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gminbampu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gmrtakeea.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gzrqwlnul.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gpzuceosy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gbewnaesv.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxkihzv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/ggzbqzyib.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gjpopuaah.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/guderglms.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gshjdkcci.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gbqzgntgl.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/grygcxqmf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gtuwodixi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghddcrdqv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gockvgrub.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gdogwykuc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gpgfqmsec.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goglximuw.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gyxmjbrpl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbjxxcoeu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/galuqevhi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyccitqkj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/ghuvqdgwj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/ghwyazxhq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gtfvpvzwn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ghtiwdzga.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gveqjqilz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gcytbqace.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gadmdewrm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gibxbqsgz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/geaulzoyd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gawbfchho.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gyfjvkdar.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdvurtlao.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gidwhimpk.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gadnqoklb.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ggrpsuazg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gklsankgp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gqenjwtxe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gqyhnqcec.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gizpjtyqg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gbzbpqogd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gfkxmmssy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gseodnfip.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gfyhvytlg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gfsgijmgz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gcanlmkic.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gwbagvxfq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gykivlupv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gosrvoshc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gczkoddaj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvxphdrsa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gydjszwfh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gedxpzipn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/grbgcbbei.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gyrgeedit.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/glvlwgzji.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gvxfsetrs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/guohdvrjr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gexmdihgk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gpkndoyqp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gqqcquocy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gwywkpizq.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/grbwbsola.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gwydxiftu.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/grkbfwpwd.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gasrxyekz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gcbzyryjw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gohuzuzwp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gqiqnsxip.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gimgbcoar.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gilmwusix.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/ggkyzcedb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gnjhyljkg.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gftnjlqmp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gvlzniojo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gytzqjmiu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gkmneijxy.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gwixxiwzj.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gnkwezouh.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gauimwhqi.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gegvpklqj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gkeaplkjn.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gwevwfqae.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gehcnbzvb.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gmbpuvgoj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gttmmwhyj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghunkdnqn.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gqtmagvou.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gngvffvkb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gczzplbvq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/guilmonwo.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/giuiklqwv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gudfvvuys.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gkrfiikmm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gvqxgykjj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/genllykle.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gtrihankp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gzavmtnjp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gpokhrupu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gmpedajks.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gzlopjgfe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gephihcln.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjyhiqpn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gtxjwivsk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gavtuvdhw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gblrkowdk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/ghocbckti.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gltppxytn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gkmrzykbg.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gokjfkmyb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gjfsbjeud.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gpbxowkzs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ggxsesgnf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gdxhqgltl.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gyghucdkz.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gfmjjbbyi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gogiprnki.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbjdsaxdb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gepffbnmg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gcoqtkvaa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gcyfobath.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfjdsxeam.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjkekdzzc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/giyizbefx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/grvanhpit.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gtuaaveom.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gaaksaevc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gieycizqp.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gdkajeubi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsovjksen.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gerllonto.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdiyixcln.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gqsbtkqll.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gezyepmul.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gfhbalykn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gkwpxycxa.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gvbhixprj.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gfbizybwv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gencczniu.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghvktiueb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gfkghzbhf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gnsrllxba.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gmzpkmqzo.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gctvqjhrm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gfrltndee.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/geuxugtso.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gldghjvyq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/ghzpmzaww.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gixqdlihj.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gnlxmqasb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gnurdfshs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gomrlgnik.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gcwdakmpd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gnztzqhwj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gapxigkmj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gyrphpebr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gmvlemqcj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gfkvwqsmy.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gnwbklllg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gpqpyjbtq.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gsgcducui.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gctjnxvlu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ggbbyulel.sHtML


<!-- 参考信息 -->