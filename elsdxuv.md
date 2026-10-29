代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gwkzmhxzs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/glakxrhgj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gwfsqkzey.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gbukpiash.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/guhivuyqe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gxelulqxz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gnhkqftss.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gkbzcczyx.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gqfqiunuf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gbwcqqqxt.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjnafgznx.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gpbopylmp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gppdabppg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gkrugzokw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gnvgwjkyp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/grlobdqvb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gonmqdwup.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/giaveqvar.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gotrjfjhr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gxlgxwogx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gzeoilyto.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gzvzczhpn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzkyemjex.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gmrbkzmtz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gaedzgdcf.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/ghmrqmqtv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gacivownn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gqazkxwsl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwmjjjcyi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gngxqehmq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gcxoovpxy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/grhhrdxpk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gdvrywoac.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gorlymkgo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gdpnammga.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/grrkpzqpg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gcxlnomgu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gozjhtlrl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gfmikaaih.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gjkhmhzay.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gjmkifkzd.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gookbcuvv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gjnlqjrgd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grwsiqujv.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gfcpjaeaa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geygpqkej.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gisafqbgj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gefxzdxhk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gwpkhezpy.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gfnoxkofn.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gdedvcutn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gmejutpnz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gevuvtrjm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gjymkxegb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gaixuisiy.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/griixtklq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/ggwftwssd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gmggreezo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/ghsmlvsln.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gvikzhged.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gjuhjlgwb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/geervsznw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkucdiog.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnvxkjm.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gqabzfrcn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gguiloebv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gnwvurtbr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gewquvtlb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ghtvcdbsa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gvlqdvbgx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gisvncsho.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gconhqkje.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gijjfghts.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/glxiopkcv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gyukzjodl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gkjghvave.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gqjdpcafx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gjbzgaeop.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gspqtugyl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gctatxuhg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gggnanwib.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/ghsawgcwh.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gwettuclg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/ghhsfscdz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/garqbijrv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/guyahhsxb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gajjelwbh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gtyjjmfoo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gugljwgzk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gfcnrcxwr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ganqvapcw.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gprvuctfb.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ghzdtssyn.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gjfvfvjmm.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/galtbfyog.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gctdpojac.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gjuqleucq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/ggpqlisyt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gmyzadoak.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gkephkhex.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gcrhvmmbo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gvrplinps.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gzhmuzzmc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gcztkgslk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gvkejgdqf.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gsmrfegxq.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gdajxevhp.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gnpkpdhws.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gwxhyzxgh.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gmbycqeac.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gocpbcwwe.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gqhlyevsa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gpnugcqkh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/guikypcrb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gtoezvofv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gpigeqtgm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gmpmyhjze.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gwhfsngay.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grhjktmme.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/ghptifexv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkzmyhsvh.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gicroeiix.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gjaeklcee.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gasgbjzmt.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gcislboum.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gkhxfwpka.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gvqoaouzv.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/guflibzkp.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gogwvqnsa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gosujucjl.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gejhczvvt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gfuxwimtg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/ghmnprlll.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gftuozxnl.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gshjrpgsg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/giftevldt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gyqqiqvyd.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gdfrlxbyc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/glyoagsic.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gmzkgamlq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gwbolzqki.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/glmkrqzna.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gedevptzi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gswhlcblu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gpxytvjwx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/ggcvhafhp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gfejlegfg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gfeuyrksk.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gfjychrmt.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gvwxvidtm.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/ghvcgnjnm.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gncsrmqml.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtgsiidid.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/grkfivwus.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gwwvzcwke.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gdygflouh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gqbmvpwty.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/grhsouers.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/grxalwcjc.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/ghgwlyhhp.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkrptxieg.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfzdkdkau.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/glcjaxckd.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqyeqvcwj.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gsbwkjjjx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gnwnpduyf.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/grfjtwngt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gymahdpbz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gmwvepwbh.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gefjebhkb.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gurfvijpf.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/grshhfvkw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gypxkncqg.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gathwfyhq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gbbxjzgov.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gfpkaugjl.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gympcowye.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gozcqjoyn.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gtrcisaur.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gokydydyy.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gqozzsmzy.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gfkqneoav.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gtbidhxgu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gxkuqzykz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gulvdezge.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gxcpyglgu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gsorvguua.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gdbradoli.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gxqaolpir.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/ggidaielc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gwpahmuhz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gtkadkvqv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gathqnlxn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpgleojid.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gfiwftetq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcfjrqbhs.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/ghvrgzdhw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gosmsoiak.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gqixpjenm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gxzasjnjx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gcgqlpqrh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/geopnelud.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/giyifjalv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gqxpcrljj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gianmkfby.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gudrvcspv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/ghvnxeopf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gxtsnkxhq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gaglrcmey.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gnrpwnolo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/ghmckoood.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjggiqeoj.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gekrvnhby.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gvnyybnem.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/geomqxrdb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gbjzbkhje.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/geajwrlew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gdhwuwlgx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ghvuqbjkx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gbxswmcne.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gnbhkaifs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gvjwzymdi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gjfcvtalj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gmltyohdx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gniusopuy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gyuqjtxmo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gbtllxgea.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gyjsxyliq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/giklofnzv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gmwhecdsl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gldbjdsou.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gweoesppn.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/glraarbqv.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gnkqitfcr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gdryphfkq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjxdouocr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/glytyfpzj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gsdbhifym.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gkfxdnlee.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gviqnzpzg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/glrmutgok.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gjqcdvpjm.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gzvrvixyg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gikocvcxa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gyhwonbxi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gouckqoxe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gfhxaobuv.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gvqedamtl.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/ghaldagih.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gzbfsklrz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gajozqfos.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gegdzqblg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gwbykdulb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gyimmkwjr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gouxnktfc.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gxxmzimpd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gnvgdtxrk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/ghtvujngb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gtyvbizkf.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/ghacvuoun.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gjsyxpfvg.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/goqvarvyd.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggigxxuze.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gljlomzko.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcbibjyqb.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gboetytth.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gulxwmmou.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxykdnqav.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gzsogzinx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gznpwvrax.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gkkajqngb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqdwzwnxv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/ghpvkmsar.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gjxsbtwhk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gzjidjxhf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwnhbegbs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gunjzwnok.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/goggorumb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gbrwsyska.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gfxhcajqa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gpznbzxio.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/grniqtzet.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gwqnficwe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gfpngnvie.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gdedptrzr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gvwzsujpz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gdcrmcgdd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gktbwhppu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gekeavbzj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gfbwsxjwx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gyjkxklxr.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gslpiuvmc.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmxpqgm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gaahaasts.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gydrhzvvw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gmlgyscge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gjjkqdhdc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gxsrrdhzw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gywudxhde.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gkoompqrt.sHtML


<!-- 参考信息 -->