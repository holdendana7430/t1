代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gncvohdtg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/glhbjjcrj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/glznvlarc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gjbrwsgyp.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gvodjrcrr.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/glmjyejsb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gqhpamnnm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwwymjabv.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjfbqgzkd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghkuklczk.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gwqwxkazp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/goezbqxgm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gitabeoai.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gdqawtvpf.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gjwayfusn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gqcwmnowo.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gvxlwjivm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gkvyvtckf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/guwhdkhju.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gioiqegfm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gxbpepdot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gnpicqina.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/guonjtmla.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gknajdbei.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gahhaufmt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gymzbxfwp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gpdsirgjg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gxsrtlfzz.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gqokkpxjv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gunmnmflx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gaohvomcy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gxnwkzzsz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gtqbsaygc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gmonghufs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/govmjzbjw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/ggtxbtfur.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/ggnvnjida.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/grtdbhesc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gucqpsdsj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/grswtveuj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gsdwhbgnh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gsmxcrayq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gigfnvbvh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gprptvutw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gixlhbgzc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gdzretwcd.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/glkdnnryq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gvbdmhkrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gtwvtewjt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gdmirjrtg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gugvpyyeh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/geuolmbsc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gujthnamn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gvkkqokbg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/ghhprzlwn.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gqlmmpbgp.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gpqoplmnm.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gygsuzuad.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gukowosbk.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gecmcusol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gixarsrci.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gehaqdkpm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gtytwmofn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gcdjosztp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gaqqvalub.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/giuumhbpx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gntbxixsq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/ghedcldzc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/glkpvdpes.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gnrujhtgg.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/guktfjlbs.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gkntqyaau.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gqoppageh.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gtczeiydi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/guspimvnb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gkcdhuwmb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdjpkrhxm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gbnrdtyky.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/glpkbljpi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gefhvgpvx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gesbrpjbz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gmrrvfoez.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcpygmron.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/glwlrcgus.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfrcbwlpr.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gawqyumjc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggvsaadac.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/grmpjtsav.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ghfitjiiv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gluqrgpro.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gaoazgmle.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gygcihhjd.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gxwqipvxj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gcvjjkmoz.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gavvjvfth.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbsxeonbv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/grwurgxpl.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gfotflgnq.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gosfgtqwn.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gluqzmvsj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/giteshgcb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gxeugafal.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/glafzooaq.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gcjiubdfs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/giwxgberb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gbdepeput.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/grbdtafpx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gwnzeeepo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gslobskyn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/geoxcinso.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gntniudpa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gztjglcxk.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gmoejvgbo.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gwfjuekal.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gkrwiimov.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gudqjnhkj.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/giekfmfnu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gveisaafd.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gvjlmsinh.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gdnykmjtq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/ghcrizhxh.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gotsbfzvv.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtglcqfvw.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gzmcdvhkl.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/geattlkjt.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gagxnyvvx.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvvtgonni.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gakccbpse.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gkdrotawb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gdadzkxnw.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/ghrdnmllu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gsceqrvwy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gqfnarogf.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gfhbzlgmi.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gcraccxkb.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gvbxeewct.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/ggawrtqjc.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gtjlncaak.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/ggymzedam.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gkrmktkmf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/grpzpuqix.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gfggwqkeu.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gmcxrwuez.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghbvgklmo.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gfoapklle.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gcdlcaxco.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gcmhfaxke.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gjzigjasq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gpjvetded.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gseochjgi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/glzgsbhiw.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gpjnjprit.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/glkgwxgqq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gkkoatqwp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gfaedrurc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gtqnazmtn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gzkvycady.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glykhyqgb.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gmgdynxng.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnacmvwek.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gnnrgyvyc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/geannxedx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/glbazrqyy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkdlbdhpo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gnjnvzjwe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkcmniwmz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmdiovgxl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gbglcrrhr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtnyocjtg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/guxecpgzo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzoxakkwc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/ghzfekasb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gigsdenhk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ghzolhwlk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gfbqbkaax.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gdtckoziy.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfvmgcliw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gmxrwfrij.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gkrgytftz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfsjemlyk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gfeecytie.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gepgwaoyr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/geiapmlhi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gnxhuicby.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gibznhzce.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gexrjmjkt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gmzlbednt.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gfxyjzwwz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gjhjspvhn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gipexwlkn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gwnflxjqn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwocbgcjd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gjxvvhrmi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gcxkbbywc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gdmjtsyfa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gaisykwup.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gpkgmvrbc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gzwuehwdt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gwoivqets.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gseqtxiry.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/geykasbhq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gvvwxbfzh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gvlfguwyl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gugaxuqnc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/glzlflyjy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggqmucpmf.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gsdyddxwe.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gvyrfsbyl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gilpyeuhi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmeniudwz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gpjwktvwt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gqfjtbnit.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gjuigusug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gsqtdlivd.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gsbqdwzpj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gnzwvurqy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gxuvlxgnz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gqndmwbwa.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gmwvpitkz.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gvzjspupj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gwyonrkhz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gmqxgjycn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gzyxuzfpj.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gpocotuxg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfbkhfxhq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gixjrddbc.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkwtmrbka.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjspudxbj.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmjhsroyg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gavxfibcu.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/glrycjpti.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxqtnncfc.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/glfkspsmu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gzyhoowhf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gpzmrgbka.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glmjltcld.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gmcwsgsud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gucmngsml.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gudqpmjnh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzywaegak.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gjuxyuqcm.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gzmpgydob.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/ggqajkxiz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/ggbpwxxyd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gkeghghot.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gmaedxpuk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gdxyfjuwc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gxojaqnvo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gqvlnebft.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/ggyhaxeat.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gnapaehsw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gdozzzran.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/ghpisgomz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gjxaugsrs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/grijqrqtj.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gapxbquse.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gfvpxvfrq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/guficnouu.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/guwyqdnsm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gipnciiqw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gvzjwpfap.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gertnjour.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gthfjmghq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/guyfwfmhe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gsectusus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/goqueiowr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gmtxkzcim.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gsbmvawbk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gggegnrun.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/geialsqly.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwdtfzday.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gdtdfljvn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gloscmbyo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gkllzesws.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gfysdmwaa.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gecpiacpn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gtwgnlvym.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gxasouzer.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gxhnwpwtt.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gqqsxrydb.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gycqxgvoc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gbxdiyilr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/getdjvvda.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gbdhudgui.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gjagkczjd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gtsdvcche.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gbuusvjzg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gfuipdjpn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gjvpzkcuw.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gqjtorhpb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gsyeknopp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gxktwcsmq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gxogpcoxn.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gosneaaoc.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gfbneqawa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gdjeaknma.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/goczsgrpt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ggsxywinj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/ggtzhbbgd.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gpaifycqb.sHtML


<!-- 参考信息 -->