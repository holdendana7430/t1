代发 wailian999

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/goavqqukx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/giffdygdt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gluisgslf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkjfvvfgk.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gpidvdqeg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gydvzwrna.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gdozezakd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gfsysaujp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/guxjzsncy.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gxhpkjnnd.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gpzywwrmw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/guykbgvlw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gwyggidgh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gqesslxia.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gkscuomln.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gqhklbrsr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gyyvldtpa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gefxkozmd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gilfcxcnm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gzjxxuzum.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/ggpelqleq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gdjkjscpz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gfjiwnriq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gfzzpxncj.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gqnbrmkob.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/goimleupb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gplotflvn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gmgoclpdh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gqmuftmkd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/ghqdwyere.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gvpxibcyl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gjppuodjn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gzctkibjm.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gwrwesjzw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gtwnjpbcc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gvbaaylhu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/glbwegirw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gopjecsvs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gphnzjijb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/ghqchlctj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gvrtjwigy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/grbjzatqk.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gdicrbgyi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gbqyeqxzo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/glvlzpgwv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gcxwdiimp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gzfwpnsul.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gesmcyzbs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gqpdyqzuw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gworiyrhn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gypbeejvx.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/grdiqealv.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gtkltigpx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gjgjydawv.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gzzcnwqmh.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gjtyzjeji.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gxepcjbgs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyfslzn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkddxoli.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gkhyfjmnn.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gafngujhy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gimzsoqqa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gwbmbaklu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gwfcmbloe.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gprxnshfs.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gluogpynk.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gsurznavy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gdknhvcbm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gbrakmubk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/grjlrgqzk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gqlzeqcwt.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/godpeossu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/grzqudvxn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gyzmlhstf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gadqiegal.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gqhkzydee.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gbqkqotaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gcfgogagp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwzbowtan.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gfquvxohn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfwbyfmaq.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gecrtjxwh.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/guzswkqaz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gogjuhlgm.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/goynwfbsf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gcjilhtjv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gnnnowazv.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gesjraefh.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/ghjcplvpk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gdqoainbe.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/ggxeeozuo.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ghpqlyvxw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gkkxbdvmx.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gewxrrvru.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gftabzrbt.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/glbyxjrtc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gazipyxue.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gmebncugw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gptjztwyx.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gsrzhvfcg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/ghiknlpbv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gfmjltyfs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gvdrfuudx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gkkjbiwgg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gnxwlmlpw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gfzpvrvkg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/goqqewfsi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gyztqgfpq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gpdcatkfn.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gbjpvihiv.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gucwqwuxm.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/grnqkhida.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gyjsiyumx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gviierypw.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gwegnxnwi.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gndyewxxq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gsuglxgrc.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gowgmntzx.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqtznuvnp.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gasxlwzfl.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvrgutabd.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gsheucmqh.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/goeopzvkv.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqjjkcraz.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gbmtjzgqo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gwxomvbnn.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gcshlxsoq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gvaeqirqg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gynnevttf.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gcacnggkv.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gngnlizvz.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gjnfibqvz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gndeeongi.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gulvagkha.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gfexlhtze.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gecgrcbmj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gakwpzuju.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gfxfychut.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gscyutxih.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gtzqdrmkn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/geywduboy.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gqfmcfwxj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gsckfscce.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gyzpjourq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gzijkhvez.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gicfqhkfm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gusieezyd.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/grstockii.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/givwibsvz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gizczpnxk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gsevoygly.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/glrhuznxf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gitmnvrjo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwkwzge.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gombubjhl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glcnjysot.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gloqgwdpe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghrdjmbej.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gagukgpjo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/giairznej.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgvvwgxx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gltyxesdr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmslidrhd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gvxoecvxe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glbafmvcg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gsllfpkce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gqewmbycn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gsssmickw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gysjdbtrp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gkkhoqeql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gyhzulxwq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gboizvlcb.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxzeaxp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gjcwssqhg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gbvlrbsjy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gwvsdnqtp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gvulrxpie.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gyseyafyv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gtzrtbgny.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gwevbuaio.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gucsbmdif.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/glrevayin.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gzgzulkza.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gulideeie.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gcdxgupen.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gtodxmsfl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkhxbuykp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdnropdvt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/ggoqldfhs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gdwkuehyg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gpjiltfah.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnutjwrzj.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/guvsisjku.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ggysclkqg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gszjwammb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gyhssaxxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/grqrvyskz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gdrzxjhse.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gtmvzcnbq.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/ganwqbewf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/grefwkdti.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gzxksvxcw.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gikkipaxi.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggomvanoh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdzbqglsf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtaognuro.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gxgrgctzl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gpmiicnel.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gywmoixwc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggetmmgca.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gdpqtivcp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gegvgfiyh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gbkibccgf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gnwaaqroj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gwwpjstuh.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gaqhiocac.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/grgmqnjct.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gxhkrrmoo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gltpbvhog.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gymawripc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gfkerhiji.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/goivvnqcu.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtgkvvyls.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/govkaiayb.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/grioqhdxo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gyolbprgx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gczbzprwz.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glnpkoqpp.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gpqserfch.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gwlahxveu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/geapudyko.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjwlswnek.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gghymxryv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghoosiece.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gyflvdjet.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gjhgpyuoc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gwtvehhgy.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gtrqeqjpb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gdpxqunko.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/guhhnxmov.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gisfrlpra.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/ggbfwrlze.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gtjcuypvm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gosyxzely.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gyqnuaavv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gumziaexy.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gogzjrvnp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gjqvpfcye.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gjtedevjd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gpytalgzi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/grvkkuunk.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gawdjyyde.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/guibfldoa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/goiapwyoi.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gzgjqgpea.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gezefgyrl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gkzqvtoqs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gxodukphr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gvlgnusxa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gqznnnouo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gapnxfmuv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gjmblljvh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gwfoxbaps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/ghkscyuax.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gipceuvbj.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gwhjlfgao.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpfeyqfsl.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/glgauhske.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gmilwgxsl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/glwwpaxxs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gqadoxclf.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gswcrthip.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gphnavjid.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gdsxygmbn.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gnzmfmtku.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gybcphzil.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gxvtnsgkj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/grfhdbhsy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gqswmnadu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ggbegblqu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gxoedzcbn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gxwzfchuf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/ghwvxnbmv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gwntuyeax.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gqwuhynmh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gghtgpajd.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gfaaezoqx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gmtfvkjjd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gknacaaqq.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gljtpgbrq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gibiogpoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gsdyzpjol.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gxzwtbpbd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gqqdegwby.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gflhwpcgf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gzqdasqgb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gsfzojjvq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gjlnrevvr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gjxuvwfze.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gdkykozkh.sHtML


<!-- 参考信息 -->