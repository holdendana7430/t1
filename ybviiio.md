代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzpnqazjx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/giakerbwl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gcpsdweqg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gsesueyrw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gamaungdn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghfnllbgj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gqfyuizex.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gepgexvhj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gnokrnycp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gsbzcqefb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gqdzlbeqy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gimypltct.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gaiimnegf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwsvhmlcs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gjsldimop.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvjqbpvya.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/geehmdrgn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxbqevlnv.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gtaiueaku.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gwbvmrqab.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gcpcaimjt.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gefojrilj.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gzqcoivuf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gfnrgnznu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gxnjjuaju.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gsnykhgnk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gifhrgzhn.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gbtolgqpt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gtynmsugg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gztijhnyi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gdpycmwpp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gxhevsmnr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gklfilfpy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gcqiynrlo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gyvqfogqx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gptjsbqyj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gyfetstea.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gjvbmgywd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gkovvltfh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/guaibaztx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gfxpylzkm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gnagckbki.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gfakuwjpv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gvacfanpy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjwqomrde.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gwxfaivcu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gktngjbak.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gbyyjhfvm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gylkukhrf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/ggethzumz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gsnyijmmi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/grnzoiiei.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gfeiciaxh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/galpeejrb.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gcaasghig.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gtwrkrnej.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gbwedefzn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gojpmuder.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ggdyfuwjq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gtxvaeord.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gemabrwtv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/ggnaegdlf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/goxnzjmbu.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gjcxdzmxr.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/genherult.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gujcygbhv.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gkxgacbbn.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/glddechcd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gkqqwnjeh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gyteoeoxm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gcqdhedoo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/glwwcvgje.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gnbzzbqio.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gmsrlajfo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gqgjgnoqq.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gbclvlbhz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gxcsanaod.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gysrwszmd.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gxosgmhni.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gvfxosywa.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnhmbyicg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gizecvypc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gbsgjpfqh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gcxusmvjj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxhjuswlr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gdhxuscdp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gzwigkgnj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gstrnlnre.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gywtudpps.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqrmuttot.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gctgxgbzp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gevqjhnvx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkwappplb.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gdwafhnje.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gnhwlqtxr.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gerriishm.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gztspkeqb.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gvcftsxnt.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gdnuiuafx.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gxjpwxyjr.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gytmcchbp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ggenwaymf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gcvsmswle.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvvyclrjt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gczzwucsd.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gctmnlyhv.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcytkvacg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gnzcosddm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gpmiztmqs.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/grpgozunz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gdnsomfxf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gtunzxkpc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/guwhjiezw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/ghskeyjsr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gmwtkdjlk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ggqozijzy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gxzjtorpx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gggxiixvh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gznkanxtw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gstsapixk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gggwjersu.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gffrnxvzy.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gyvkxmvjq.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/glwxnerea.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtaesaohi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gxtyxuxuh.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gzwckwgqv.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gazjuncwf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gtlizrkzr.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gkftwuzll.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gejdodnxt.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gdulzmavp.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gwmqkouif.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbovmtlht.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmdlyfgyt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gemexvkve.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gavofjrle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gfgsybjis.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gdxckjxct.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/ggndbioii.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/goelwummu.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gqfubybja.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gafpnzhta.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gszbkaxgb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/grqpvxwlo.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gcfhcfitt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gqmycpmrh.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gujtsqwuv.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gojjlfhbw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gwfuaicjq.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/geywlavgj.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gfepqkyzx.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gyndvgizh.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gduupkejy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gslhedixi.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/ghkxetbtq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gklecifal.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gyvznswrr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/glezocefx.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gjzijxzlz.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gxsefxasx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/ghknkqlkl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gttsfpvca.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gzidulvlv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/glzfscwir.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gouwjllpg.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gftrvzegr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gifreckrp.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/grdubgnbd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtkrqbvwy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/glxcqxjsf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gkpqlqmcj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtwyqzkbn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqlmtngot.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnffzvcdn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gbcbdotzk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcidjovil.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gruommksa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/guonwubvr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gwfktcpbd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gdsjkbjzr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpvzetble.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gqvdwhhvg.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gikwkeusc.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/guoytfaga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gzfayxzuz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gnnabfmiy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/ggbdukvxm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gmmjsuubj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gveomdllj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gpzaqsqhd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gafdqxtja.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gelifarud.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gqqggoksp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/ghirqocrz.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/glgyvdmzc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gmqcnoivc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ggpjzfldd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gxszgkdwa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gdjupyusl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gkrsjjzgh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gaxubtpsq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gwekwbosw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gudyttngq.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/guwxeowlh.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gtrgqgugy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/glrsiuygu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gzzppzcxm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gbbktubcx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gjpskkdmi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gywcsvfnj.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gyiwopslq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gwgchjsfk.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjazrrkow.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gklylcdwg.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gzkfoxfpu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/grlgsqqxr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gwrcwpqxr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gyjbqgveu.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gbifvpzba.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gbdhbincr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/glmxfrila.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ggniipboz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gwworawms.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gvqyybcrp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/goqxheqnj.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gyxuxszqo.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gtswzwzzk.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gqrgyviau.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gnpljpfgj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gbowabljf.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gdvroyncw.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/giwhvmtze.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gdejpqksx.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gnrxgzsps.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/girewedul.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcttdfoqc.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwtqzdloc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gsanswucm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/guvvtbvnu.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gqeubbcmd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwaynbotu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gpjrfoszo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggkganhmm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gfwzlsrxx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gmeecpiej.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gqqknjawz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/geijsmfxk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gmazgscfe.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gqqmyecdm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gwsafpzgv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gzkldiits.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkvrdzzlb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gmrgbyruh.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gwnfazymu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gdzoowxht.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gtyqlkflw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnbvbelf.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gflkblzph.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gjgclyrjd.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gxobrmiys.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gpymhwixk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gngasndgy.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gpkihqanq.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/grprzrtbn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gxhnacaio.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gidlvqgqu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gmojknmxa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/guidhdhjx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gacvmlroy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gdomnpkmz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/ghjmvynew.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gjhjtvjvk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gzseqdqje.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/ggztvtjdy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gtnszlovd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbzxygugd.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gjcgtehrj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gognrcomd.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/ggolamvmw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gzzkwusdb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbypsjk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/ghmjhsudy.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gqpxnvcik.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gjcwwykok.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdukxknjl.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gbqdnhwwr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/goswwiytu.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/ghhexaxif.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gcmcikvrt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gwvazscgw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gpcgyucyt.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtodmib.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gotyejbxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gofvlmtss.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gdhywfdxb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gpqpixtzc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gjowmsnug.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrdpbmf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/guvuybzkd.sHtML


<!-- 参考信息 -->