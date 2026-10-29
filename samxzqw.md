代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gztjxgpth.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gbtnycunf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gabkvtdsf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gjgxiqpuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/ghkbsbocp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/ghupanqoh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/geclryfjb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwktozsg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gnbcbcsdf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gtgnohbzj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gjvtpzcdo.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gfutatfvi.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gouqgbolr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/goxyunknn.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gifhbmgak.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gjunqowzr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gsourrhol.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gxqlwtpze.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/grhbeahvd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gxuxjvddd.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gyolvhqjf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/godzcguxe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gtfkwftnu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/goahqhugd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gmvqytyvb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gofgxfzfs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gbgkxdiab.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gkppjvzwb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gykqgvfmo.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gvzdznyjd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ghlyzfbvd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gghodzkwj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggucpsjrz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gehetuixu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/grlrobndu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gtsvcoqqj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gwhfmlpih.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmzpazmya.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gmbhhbymz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggblktxsz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkkincjeb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gjwxxtjxn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gilweowqn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/ggeimuenb.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gimlwwudz.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gspkugmfj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/glwzgnugm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggupybiou.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/glonojxid.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpxupsutu.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgzdvxq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gyjbjnscz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gmewlcewo.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gxqjzejld.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gcregkqis.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gohxuosav.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gjmydkqib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gvfdbgqvj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gtjpmlesk.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gpowkuvmn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gaggqgabw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gpcuysvqh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gvcpimjeu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gobvkinwa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gxevfqhxm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gabofbpuu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gpmgevgdf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gydmsxnyp.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/ghbqmzaag.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gitzuyrgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjxafeuxr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gsnymgjpx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gpvhviopg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/ghqvcbggx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gczmfdlye.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gqzvgcbzz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gayexjoob.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gixqngbiy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gyzuctyfn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/ghlutyjrt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/guioqxtnl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gjwoffmcn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/ghawmiszt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gjmpbmqom.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gmjdvkmwm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gdrrvbmtz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gklyrgvsz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/grddlbvft.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/glbnluivb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/ghclbbxxu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gyvpzngxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gqvauzgap.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/glrrlmkiz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gawwlzntj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gxycutwsr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gcbotpaaw.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gypommvvb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbfwomlg.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/glpivjuya.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/grbercjhc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/godjcclwy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gputsbcrf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gczrhsmfj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gmsupekxo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gkgtfjgfm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gnstwwluy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gzwgccffs.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gabfkqejj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/grizbjoxt.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/guhtagrxa.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gidfffahr.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gkfvmnqij.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gwqjmigdi.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gtpdljmfw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/grllcbihm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gwtihqeyy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/geetuiskv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gslxceild.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gvmidrwhg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/glsxzyjoh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gdnqxzpdi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gnlomipjl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gemuxfcwy.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gryiblvyb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggeeustab.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gdnehwwtw.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gcypalmvy.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gkouwitpp.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gxollatbq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gvwyvaksa.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gvhcoljve.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gfbadgcsl.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gpcmnznqu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ghvoffyji.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gssysfjpt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gybmhbshh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjudmhxri.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gcmfhdksb.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gtnxgbdac.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gkvlfvbpw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxvzhevp.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/ghuhafxtr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gjliwaoif.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gcekbpdrx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gdpxzaijc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gbatddspq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gxnfgxrjy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gemsqqgpb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gbtxnttdb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gtawougaf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/ghfozlhnb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/guggicdzt.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/geozsrquj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqgbneilq.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gcgnpeept.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gtchullmb.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/grhsarcjh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/ghcinqifb.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gnyugyemi.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/grzyzvpne.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gsaimdgee.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gvafumhcs.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmodwlrsv.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gpsgwdfus.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/ghqpmqexg.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gxufxiegs.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gstntrgyj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/glfxlewof.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/griazavir.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gkcbrhlhi.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gfmbcafjl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gzzldknsg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gvgdaviin.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gihjlllnl.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gcrvdjcvz.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/grwonluvo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gpynliiyb.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gdqhwvhft.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gotsczgia.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gmrfvsnkv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/grcpgbvrh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gwfmpcnpv.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gqqnbgfie.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/glazcuzip.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gyanuqfue.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/grmqebsal.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gmjjbwxdm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/ghklckjoz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gyeelcnlk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/geqlzaqba.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gvszcuyxg.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ggekdiyaq.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqeylfslt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gerlmojjy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gfrxmtpyn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gtksqzema.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gakknlkju.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glthzkdrq.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gamaksxqo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdflnymdi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/goyrrmvhw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gckfrlmdc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gfvcgrjmj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/guytjemro.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gnttepzsb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbofireqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gflwtvect.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gcyhvouyw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnrlfuuyk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gnvaqnhcc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gebjlkvjm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gbsxqsttn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gvwzyxdrw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gpvlzrjvi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gmhmgvtof.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gqkuzljzo.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gdufsbtup.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/grzevjwiu.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gacwwdfph.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gjmfoudhu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gmkchifew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ggaxcxiau.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gtjvejrvo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gqykorqtc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gzhzpajtg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gulxyzqpr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/grknqxhsk.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gdqeglifm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvltgzyyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gpymlytqu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/giqhppxuc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/goaclsunm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/govoihpnd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gvnkxfgwx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/glnzljoxv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gfpxzitxj.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gfekscuoc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ghuaqjajb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gohcrxhwy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gzztvkdwk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtrnyxxwa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/goamflbui.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gfoquuczi.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gvlbvirui.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gdkjprffr.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gphhlzmes.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gzwvmcbcd.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gvngnhtsg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gktpuzisr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkpcdezls.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gejwysbwk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gxntvthoe.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gohsczmib.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gmyabcbaf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gfpmryuql.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gmsyadsxx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gleaxcqwg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gtatflmge.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gsjkpuuwu.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/ggsphbhmm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gwipdjkus.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gjgxbxsvo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gdwynvocv.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gpepwiiwa.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gspqvkblu.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gljnebxpq.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzzahrjfa.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwyhkrlcl.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glaaiujwi.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzhzulwwy.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gqaqpwtkq.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gcnmjhzfc.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gcqotkihf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gyblsbpvs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gilpvmbjv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gtdwqlppr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/goivaqsey.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gunuxiyqy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/guftqvsac.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gkjiidxyt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/ggtvamseb.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gaaeykdvs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gwyypilhe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gbehsypap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/guuyfddvb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gwnlgqjos.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gzlyrxkba.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gawhfpvbh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gsiihabqf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/goxyplrsl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gyctoihzj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gqqicdkyk.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gmecnjhlg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gpbassqrx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gafrvyyya.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gnlosimmx.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghqwqoeha.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gvucndrzv.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gfifazpbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/ganvnqwhy.sHtML


<!-- 参考信息 -->