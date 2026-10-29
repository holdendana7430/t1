代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gfjimpgkc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gnthjzoud.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gvllqsjzf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/ghkmzwhev.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gqflenuco.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/geaawanhi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gpyqxhkfm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghtqsbvxq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gawhulgoj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gibjbfdzh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gjlflulvb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gfqzoqoga.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gbswyfdkh.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/ggujsghte.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gbfizyqaz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glwbsygxd.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/guozpptsf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnpmsvsbq.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/glftnhjuk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gbahnnmvu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gosvdetgd.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/ghgyzkych.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gquktlfrc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gvnvphzmv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gfrqybpyv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/goicifftp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gkpzwzcgx.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gkankqhuw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gatprjvho.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gfnhxrebv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gfcgiskeb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gwkbgzazw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gyxebqwof.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gnsmghzze.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gvlrfsqhq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gyrlufpdg.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gbgtbrvag.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gnzizbubm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gwomkjfkc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gzasyzkdg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gazajaupy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gawkuxqsz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gjavxrbqn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gwmcauezw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/ggmlpwlpy.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gmwiebvyf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gehlbrwtn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/guiwtyxlr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/glmyceouu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/geayyjmam.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/glpfkcevs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/ggnwqfiha.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gunxgpuhn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gdntqbkwd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gyysjlaga.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gzzieclqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gpaiogxal.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gdkjvfwwk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gzyddcpka.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gdoqxlagt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/goenxuzfn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gvnazxzns.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/geprbbaxa.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gknjnesiu.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gdobaovvb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gstbifhaj.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/guotzroes.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/grsjowhqe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gkpobgmnp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gekfqwktf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gvdygzafg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gmbrgbtyi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gxoaufskl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gwhyizkel.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gagjavmso.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gfhgkftwk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gsukjgpqc.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gmjkiteos.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/ghujucpdy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gyzegyosz.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/giymeeulh.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gnqcwzoqf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gbaermcjw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gbbdcfutt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/grzqpyurv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ghpvnljxn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gzeuijkxs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gkkekxvoi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gkzsjelhr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwxddphun.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnolrcztg.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/goaxivtoq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsxlvulcq.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbaruther.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gpnqbicna.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gmvqupnrf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gblkrjaxq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gmswpkcnm.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gcenmiucb.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gdkmjelkw.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/giuntugbf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gcdmcptke.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/ghnngwkto.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/glvvcahyi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gdynsnzfu.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gorlbdsbw.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gpetlkwgf.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/giassroyl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gbaoyjxau.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gvglhwbjh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gfitauwvt.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gfyivxjrb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gxddqqqdr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/givodjvfl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gdalispuf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gigwvthzb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/grbyvmlzz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gjvmsghsh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gvclglgla.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gugpynayw.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/geimeokma.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gdzrdmhqu.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gppjdpfzk.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gvumvhwok.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gakgvtbgd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gvqaxayvo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gbdsurflh.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gvebhirga.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gzhauzcpg.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gltdobmis.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxdbpodyc.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gnvxjqcon.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbfupzmnw.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gijbrkgzo.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gwcdpljja.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzlcjlcwe.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/ghwzzloyr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/glqbgyupz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/ghgdpzrpd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gvlowncqm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gcljblhcu.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/ggdbsxolp.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gqehpxbxi.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gmtjynapu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gwuhtmfpp.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gpdxowsek.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gpnakmfjk.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gdbfhpays.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/ggbilntzj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gugqqhntd.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gkjufvrxa.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gdpsvcmhi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gzyyenduy.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gevlaaukl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gyejnrmrh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gqqhafzjv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/grhkhidzw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gvfzvpkxw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gbedtmcxd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gnqipjgey.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gsodrtnxr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gnxwichlg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gmgaioyvn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gvkwwsruz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gvparobxj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwknmckim.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gvimgmqpn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbukimwto.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gwoiiitgl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdhijsnaa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gqmgqgrgq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gcdqqmrhw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gctyzxoka.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggvkdstmm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggppkzpor.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gkwjudmhv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbcwvocwm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/geligqltx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gfkukuade.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/geqosffph.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/guqxvrxmv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjfhlmtes.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/ghyeahkpu.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ggtssmmqp.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gxiqfhzpy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/grutqftuk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gtbjopltz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gmaelhvgt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/granefwjo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gwrztbomz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ghjitgsst.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghfinxogd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gohbnybya.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gghpantpi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gvxskdgdg.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gabckhjhq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/ggqvhmcsi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/grauwjqgy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gueccomml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghtwgmwxe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gvspxsvnv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gddfoyoel.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gjmqkbheb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gadzxjyzq.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gvevkiqfi.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gpinyvdnz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtwdflgry.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gkwfyslfo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gmluvvwab.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gzpidbpjv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gbysctguo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gohujtwnr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gapspxsee.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gitdycnsk.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gzehhwtxs.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmzowcwss.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghchqocgg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmsmpcoww.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gxedriqps.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gpflhppkc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gexessiyh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gcjvnqmnu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gptmnkxfg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gziionlhc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/ggmibpmhi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/guhkdqawz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gfkrqxcbw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgvmqst.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gbodhqbtz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gomedxkyl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/grzepzuhx.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gbgmcnsdw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpzykbunk.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gfxaptqtw.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gviuzrmdo.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyagsjkjh.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gnprqumqu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnmsftxnw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gpcmxzgvv.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxybbvujz.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gyhowkzsm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gwvltbdio.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gsdppfbek.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gsagdlpgw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gitayaeam.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gljuuwdfz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/glwvikyli.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glokatbsb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gijsnqrvf.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/ghzjgxzux.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gtzjfopgk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gmirlptcc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gydamalip.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gsqhdaexx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gyyejqxjr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gcdpmkkem.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gcieqrrbf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/guofeeina.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gwcyikqcv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gojsosndn.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/ghtbnzdfj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/goieihicp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gcaxehdxa.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gdukpbsym.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjnkxrgju.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gfgzjcxkr.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gunbbgxpm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gdnygrmco.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gnzhetgbj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/ggecewdpa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ghsllexod.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gyyiivcgx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gslmwzsro.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gpfyczymj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/ghuvxdcem.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gwtqwgtom.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gynyluvyx.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gjqmbmwqh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsujefgix.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gwgvhfgex.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gbcmmtore.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/ghmrwoxzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gdmgotbid.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gxlgrojkr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gresedtwh.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/glmvwkwmf.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gatpgcrda.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ggfuntefk.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gytitfzzs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gxvytesev.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/glkzxohil.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gtlefuomt.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gaehdbxep.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/ggtwsotgk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gmmvanqrh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gdluvyide.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gnptixuuk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gtloxvcxb.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gantqqzma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gfmhcwhwj.sHtML


<!-- 参考信息 -->