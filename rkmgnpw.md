代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/glanqdjyk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrbfmnsw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhpfoesz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/gkzwpzboz.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/guatoiicl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/grfzxghis.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gzpqwrico.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcczxpzyt.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpaiwpxf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrqzfavd.sHtML

[L01] 发送 GET 请求
来源：http://blog.fanxiaobao.xyz/Article/details/gqnbyubay.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/gatrandlz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fanxiaobao.xyz/Article/details/gezlzdrcm.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gociqrpyw.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/giesowebx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gjzzttybn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyfjaooj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/gyrmtznod.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvabwwucp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzelfpap.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaflinoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmjeina.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/giiplwdvc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/grjeafatl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gqwtxwpnn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/gqbjjncny.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyqbjopz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbcjcvid.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gglkzylxz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/gdnamdxtk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/glgkizjoa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gsmblwvtr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gonpxiglu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxxnbmml.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpefnkeyg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbitsedis.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbskjlxoh.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gikwmsoxz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsvdstwu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/glevjwbjn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjyenaiu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gdxuufvyx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/guintgirw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuruiwvp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/guxichkgg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjafhxjjt.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiiuduwg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwfokgyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fanxiaobao.xyz/Article/details/gjpxekoqn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/gjsqylkkv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrzandhr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvydexff.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcturgmux.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fanxiaobao.xyz/Article/details/galkfrxpf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvdyveog.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjqzvkly.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihkwxhfr.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwovacawd.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggybafjry.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gccsozdid.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcmnnfjp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbuhjhuy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gdfnkivov.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlhjngbw.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gisvvzhlm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpegiojsv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gsivmbmrf.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/govahysay.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmlhhvut.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbmhuwiy.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gqtyjwlof.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglflcily.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gkijjrlse.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/guyudmmwy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gvnoyuuvj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fanxiaobao.xyz/Article/details/gyswfcfzl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsypjaqy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxxfjpei.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/gwdpsaobv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyeoayxt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gvfvrdsus.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpalqikev.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gydlwebig.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fanxiaobao.xyz/Article/details/goowsqqrc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gewubactk.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsozvwzj.sHtML

Py:   sys.argv[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gpzyhmfzg.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fanxiaobao.xyz/Article/details/gqyfidmdg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoorjfdu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtkcobwa.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gsceuszcv.sHtML

Go:   os.Args[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/ghordgemc.sHtML

Ruby: ARGV
来源：http://3g.fanxiaobao.xyz/Article/details/gqlmzclmw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gdqfshqpg.sHtML

[M02] 读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtzoorjqh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gkuhtkzpy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gsikmdthp.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groazdqwm.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxufcecs.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjwecous.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwssgzmx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fanxiaobao.xyz/Article/details/gibqxrevf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmouyue.sHtML

[M03] 执行外部命令
来源：http://wap.fanxiaobao.xyz/Article/details/gmfmirujx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxvyniny.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gayxybjbd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gockqbnvs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcwyijv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfayokcq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkvztce.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/gsuazkkjy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvrfxpik.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/gltqitdkb.sHtML

Py:   os.getcwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gyvvxklcp.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gylbpbzkb.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdcuztjt.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gswgnepjq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gpcvqyrpy.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gypsyovri.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gzybaiops.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdvejobd.sHtML

[M05] 设置退出码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbehlfjd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjjqtvqb.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/grohozgtu.sHtML

JS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfvujpvp.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gosykyrsq.sHtML

Java: System.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtedakuyb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxxjhofl.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gflzdckio.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fanxiaobao.xyz/Article/details/gpppxljjt.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gprarlspu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gffkqtsqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpsriesb.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gvivkjthj.sHtML

TS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfzdsdho.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxydcbpbj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gfhrljdqy.sHtML

Ruby: warn "err"
来源：http://3g.fanxiaobao.xyz/Article/details/gvzmqathp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gazdtpxdv.sHtML

[M07] 判断是否为主入口
来源：http://wap.fanxiaobao.xyz/Article/details/gegpdpklp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzzkkhah.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fanxiaobao.xyz/Article/details/gdmcnrkus.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujdtbuk.sHtML

TS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/glfrkexqn.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaipuseo.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gksqxoymy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmvycsxe.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeteegmd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fanxiaobao.xyz/Article/details/gtqrhcouu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmemzdaxl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/glpomtjvn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjjkdiml.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/giajcmvvf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwejqmecj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gfmuqsrwg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/gsesvuzpf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/gtltheabs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonrhylxk.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnfisdcb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giatzbema.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaetjivo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoeafwiu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdacmxotn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gzeeuanfd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukmtbpbe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwvqoihbk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gaepblwyx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfisjpiyc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekefcwex.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhmrvamh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gkiuihlrz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtbpllnh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gupqllemq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goysafabc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gxszctbvv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmksaqcg.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/ghjcfqbsh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxpylhaf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzfgtgqz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gyrswonvg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoklgfps.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gwolhvjdv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawqaiwfp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gmhumuwoo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/genezlmnz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fanxiaobao.xyz/Article/details/gvgjqekod.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsppsolg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibqwrfjc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoqprhjq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbigeqhp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbtlhoup.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gabytpntv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gittxzpiz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvpsngfg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjeobwnvw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gieauhicx.sHtML

[N05] 最大公约数
来源：http://baike.fanxiaobao.xyz/Article/details/gzbefzadu.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaotuwgh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grlvafzib.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwaohiso.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvchseyy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gplmtheso.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbdwblvn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gklqriqyj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrsoqlca.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtstnmfhn.sHtML

Py:   s == s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gdzazqncp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gksccenzz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gqpskkdyr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhtnyzie.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gbslbzirp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glvgtmwug.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gyddoelpe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/ghtispbvb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucfhxtkn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gvqbuqiyo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fanxiaobao.xyz/Article/details/gaidrecyr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvywdduz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fanxiaobao.xyz/Article/details/gsqxciaqi.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkentizj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvjphlyt.sHtML

Ruby: // 手写 Hash
来源：http://baike.fanxiaobao.xyz/Article/details/ggwaarxop.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddzxtbiq.sHtML

[N08] 生成全排列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhjkobuc.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjdqzgvn.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrnjxsrh.sHtML

JS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gmbrfwztn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgoagtqq.sHtML

Java: // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/grjrdlbzb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gojaupify.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gadlaqpxu.sHtML

C#:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gmoajtqgh.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gxdeiuljr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gnahlsbxi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gcplsdkzw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzyqgch.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpjxryyn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoaekltz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/gqujdcgxn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnucrjgf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwcxumwp.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtacdowgr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdduejuzw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fanxiaobao.xyz/Article/details/gblyfdzdu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gdiyxtftt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzydxmeiv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrkcegks.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/gonlhfoio.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmtdujaz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahajmbks.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfmhtlbd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnaybuog.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjrkhpob.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gytbktrdn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfpogajy.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gabzjditm.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gxdmpyvli.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvamqlqk.sHtML

C#:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/groyvcpvs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcaazpcn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/gyutabnwp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/godwsxxuz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gtiunbmti.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gblzmuxvj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/ggudumxjj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gxwjqakdx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gksgtshbt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvqtkqcc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxmkmwhi.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/gudcfsuym.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grmimppld.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/grrxllwwn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gsdqnbixw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnhwdmiu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/gcxnqmdoh.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmwnyofu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gbjvaqnxl.sHtML

Go:   go f()
来源：http://wap.fanxiaobao.xyz/Article/details/gsyhpkfnh.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwftkugn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/guxrkhapd.sHtML

[O02] 使用线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzuhdous.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/gqiftndsn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gcpuvatzd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gvduahzcc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguqxqpke.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmxsfwry.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfbgqxii.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gkbniwomt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gkvkczzpl.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyictuxqd.sHtML

Py:   with lock: shared += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gsuaeusxs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gsamlqpar.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcujiqtjk.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gkamtjvdu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggashpuog.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjakcpjey.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyzvbaez.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuykhvil.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gfvzaiwaf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/ghenjhxpr.sHtML


<!-- 参考信息 -->