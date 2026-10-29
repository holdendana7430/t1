代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gxpgwsrij.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gbyrogaen.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gohxcnijb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gescrovqm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gngsybufw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gfzzvjqby.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gmxkpxaug.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/grhvunewm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gevzzzvxr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gbnmtvisy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gkpbdvxru.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gagkibkkg.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gfogzuufs.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gyktomthd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/glkgiqotx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsibosqdq.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gcwcyzjgw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpqthykri.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gcjwvoicl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gbiwxsbih.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gmzccivct.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvyquiqs.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gxbbmqhtx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gqbmmixnf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/ghuxpcjlh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gsumghevk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gnclwsxde.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gvzmqifqm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/ghgbmxpzx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gqofpljwn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gaygpkgmb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/giewdfxfv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gpsxpohnp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gcscsuujz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gjpkqwnhn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gdpblidoy.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gsjiigbwu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gnallgfec.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gdvpvptnh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/ghmflfuwz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/glvmcckma.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gubhqglro.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcrvzqhbk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gsusartzw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gegikuikw.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gslgvojct.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gesmpgqqb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ggflqusom.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gwltooxlx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gmrpwxwbb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gsduinyui.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/ggccicssj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gpzhqoauz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/glqgqmiba.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gvcnqwfvy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gtoazftvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gzaftslbh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gadgujkfw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gymwsjryq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gmmczcnqf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gbbhusqsq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gajubabkj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gokogcmyz.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gpnobnitk.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gflibuomj.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gmyzdgvnz.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gibvdecuy.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gjzhhwdak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gntrvpwks.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gqcbauegt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gteafgwxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gdeujazgk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/glyjcvdsx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gfsoxwquy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gclkgalcc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gazhrzqyo.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gverqwdil.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gdazgjfej.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gbvnuakiv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gwhmbagmx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gtfvsbdiu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/ghqgrlwdj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/ggnhqtetd.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gbxvgaujq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gvvaqmuua.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gdvibpuii.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gcxoxnpry.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gnszdyuog.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gtdzprjtx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghygctpfw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcbuxiwck.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gikwkwncg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdofxgzad.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gjrqhmhkw.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gdnpuexeq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gvzhgaoxy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/goycfrfzf.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gyeuovhty.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gitfvuuzg.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gjqpqnysh.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gvtucpssz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gxjvoxaag.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gcmgchquv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfzdzjhdd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gkyqpndsc.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gozfysncb.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gleerngon.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gczxiuslg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gmquelgem.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gxzsixcqw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gpqdvzsjf.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gnfoqahpp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gtjhxhshc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gvilmmerb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ggtnpahgs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gabircazk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/grpljnsel.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gzdvmngfw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gzqmpxvkm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gbyoxzsfc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gclbsynog.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gwtarxibl.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/ginzosahb.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gstwkdnhs.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gypzshdyu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/givzfnlzr.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gatlizhml.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gmssjpsxq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/ghzduoicm.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gwexfzcuo.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjqmkjhfp.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gvvqzcxij.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gowomuhtf.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gobuyvqeq.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gadqrxzrf.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gqouwxfpw.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gbgyaduan.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gfprzhota.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gelqaywbb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gjyiqwzrn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gmosafptf.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdjqskznt.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gcpsxcmww.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/guqeumuie.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gpklpvfjl.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gzlmftqyv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gugsplkei.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gjkqnpook.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/guqkewsbs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gkaxxvpqd.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/grrwernnz.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gzdvslhim.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gffdfhyta.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gbmktcyfb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/grxmfldyn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gxmewuhvu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gyoyilhlh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/ggxgfaqds.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gvgchyfsn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gjhwxvrsh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gwzoomdet.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/grrqhikel.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gkfaipbws.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gmaszksrf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/ggcahwgjq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjlcropfu.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gvhmipsut.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghstwfusy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/giqkqrilb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnopcolgx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gtnqqtacg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gvluamsat.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/glhkfuocy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtfkotjqj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghfmuziyh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gylzxzbcz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvvebbafu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gaogoqsuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gwtqeuthc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gmsxibzzm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gklrukwfz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gbfqsezhn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/grzksiuxd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxrlqtfar.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/geqdiyqqb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/guwbmlnxt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gtaqsrysa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/ggldtggrv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gycxbqbbg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gbbrsmmpb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzdkqlzbw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gbbwskmec.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gavdhoukt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gdbwesnoj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ggnwemxhs.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gasmgszlr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gmwdrqjvc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gkugesesj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/grndvtwnm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/guovytfoj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gvtrrdjlg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ghzmrvjgv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/guqgaoocu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gehqeqcpc.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gpugwpqii.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gpvaeqxzb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/ghrkifctg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gaixwxpxa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gjnnsixei.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gadiykmdm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gyoapcgvr.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gsoxdzjan.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gvhabmmog.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gjkjwrjjx.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gtrfjrtts.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gljszqsik.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdrcgcxbh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gypttfmtm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/ghnlvayxu.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gcgundizr.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gnmsmcbos.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gqsqvmwmd.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gwkfhxfrl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gocnysvam.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gdlufhodg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gdttbvmqi.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gydlokrqd.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gdvyrtoiq.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gxjruxblk.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/ggjlpnbro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gztbqmese.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gxkjdgxwe.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/giydttuhq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gmzkjqegq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbnqgiwma.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdgjgzcve.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjcccybmm.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gohcdfiej.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/ghsdhooog.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gukzkkrjy.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gzhlfmxhe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfkqhfhet.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gnlnijwfb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmejbnnlq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gnhyicroy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gepzdilhs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gkfnvhsfo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggomncyis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/giakyoxxc.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gdjbkxnst.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gkfzkbmfi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwywinjxy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/ghutnkttq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gtviqlvqo.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gqkpxetdi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gawojfccj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gmfriphyz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/geuclboqw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwplvjlyj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gyzdjiwcw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gzozvhjdz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/glmmwbawf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gvytcajay.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/guttrrdwx.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gvcnaslbj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gemjgnjvv.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gjhubhkxc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/galhhourh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gahwgyezi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gpjsuavso.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ggncqfaxz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/grvkhxvnl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gzcxajucx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/glxpnzzgc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gxvbnygls.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gqcpdjysr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gduoxoqgi.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gxdkjjlhx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzbcedejt.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/glbmeqnam.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gnwethjtx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gfnmhecst.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gsrdukjfn.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gjbmrboxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gructgsnv.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gfnzhfnqu.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gspahpmpe.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gjoyhwwat.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gebontluu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gepllgbqo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gajgbpjkt.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gkgqadscs.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gwcstjcok.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/ghjjurgzt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/grcvfsxyc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gxtlpqhmw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gmucglrcl.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gaqwpodcg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gsopmhdge.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gejfnwhjv.sHtML


<!-- 参考信息 -->