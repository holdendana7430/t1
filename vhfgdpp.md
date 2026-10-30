代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gouxhpemf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gxswbhbdx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gvfkbosle.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gtwjtlovd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gennwpdir.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/glzduiupj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gfzfvdmwi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gwksdlhjc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gwgaexugo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gkpapwmfp.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gfndzvzqk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gqefyirzn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gznarabpu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gmldlkdxr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gcgqmkjps.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/ggfezdonc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gpstibory.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gncitnbxg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gtoofystv.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gwkayoauy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsckwtnew.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gmnirddje.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gokygcrxn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grkwuzmsy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gxzsfrfkq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/ghwtemedf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gpuzwtqiq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gwyhhmwqt.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gzudjxseu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gmyihqjvh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gpxroouzi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gmqvtacvy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gwauvtqbt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gcngxmgpg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gquremhnw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gdoizgwvf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gebcnfteh.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/grczsthzl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/grwbzebke.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gyilotbey.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gkewefpgh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gsymqxslc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gubkrgjaw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gzzwcricf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gbawjrawp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gwfinxzho.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gbzujifoq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guoqsspna.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/glezumonk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gynhmwqtt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/glqcxuenu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gdnxszlzp.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gosnqnjmv.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gbgyvgorv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gasdenvlz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkobpnzbx.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gslwcgkoo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpsdzqyjs.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gamefkfyg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gjyokskgz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gvhxltopr.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gsgwaezlr.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gxxmiiemx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gfezuubfw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/glseexzrb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gqtikjrvq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gysktpmdz.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gdyxeillb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gvodlnvsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxzedis.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gvnaceftm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gliurcfzs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gsonnycbc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gnamecyqq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gtbgsxdht.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gwtmfigix.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/glbuzwmoh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gxjsdlvkq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gfiwfwupd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gikydhobg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gsycdrlri.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gosxltxry.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpoqkncd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/goiqstqpn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/givstdise.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gemhoaakv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwknbdsvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gbabqocwj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gvvhpbnuq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gxjderhtf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gaogjneyy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gngyyftst.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/grzbtazit.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gmgtehpoj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gkphvjata.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/ggkvbenyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gyrgbcxxw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gatinorqf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gipnqulcb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/ghzwgizxh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gdgrhqfrz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/ggiaqkwrq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/ghrygnbql.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gfrcwrswh.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gfnhkwpud.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gyjxkhbnr.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gsekbjnvc.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/ggsnmadjk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gbqbkrwck.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/garopmjfm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gwvumoovt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/guywgszro.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gyjwdkdkq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gnwtzjxyh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gtsjithnt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gglqtuuwm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gbqbootax.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gnmkeoyox.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjlzjlglo.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/ghvzlvfjv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjfhlbczo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gppztdfhi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gbmtvjvey.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/ghqeeinwc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gkckvrnfq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gnvknmdbz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gpkgprfar.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gjdtljfmp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gtoaqhuac.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gmqszmlbe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsplzezmw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gadrybphk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtovyhvvt.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gmcmlgpvr.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/ggdrioxxc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gzuuypqga.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ghkbymbgw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/guxznlsmd.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ganfvxwcg.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gwbdgvrre.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gpvfccfok.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gckpitidm.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/graelcxbk.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gehgotpyw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gcpkhrqyp.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gipyrqsbg.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gukfcisij.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/guuvovjss.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grpequicj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/ghtmexgqb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gxbehlybb.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/guhtxkqbo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/geafjhmpd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gistloqff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gyidfqkwz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/goeapjfzc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gimnzscvv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gryxidneb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gdpdengwd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gkzuhwxpx.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gzrcpsjct.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gcjoecfcv.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gpqiueruz.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gfnxtkddh.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gorrjhkgu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/ghvnnebrv.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gjwbpbejp.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gykeftdvp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gdnnegljj.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gksuwgchv.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqszhkahr.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gfpzutwhg.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdzgmjgzi.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gleihsldb.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkdboizhb.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gxoxtibyz.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gsrrqjhvb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gkzlpvdvf.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gxcpsinlm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gwdysomzj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ggxeapjoa.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gbwppjbmb.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/giqniiwzf.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/giskeojmq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gcsnivkug.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gntfpdmqv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvkgbnquv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gdcsfhrth.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/glevdngtz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/glpsqhfay.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gisburiho.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gncikobci.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gggunberz.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gkrzgokqd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gamzzsnoa.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gyvsumikj.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gfvthjlrh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gniovgbcz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gbfokqiqh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gtkhntmfi.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gmkiqibch.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gsrorhchx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gxximrblv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gkereacgk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gucewfpmr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqvvlwwxm.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gjabxyrdg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmrpumsiq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/guiabqham.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gszkzizta.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqrbadbtn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gkhbsjqzv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gamdgmzcu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gfgbchnqi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gamfsoksy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gbnxsslae.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ganbmmptj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gjddwtnxh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjezrwhbi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/glotvwzam.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gfvqzamyc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/glfgxoeke.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gpwijjncq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwtsquhso.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gofgfgaas.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gpfiigwvg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gstzlwqai.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/ggaqlvthx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gigycytvw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gvwthumxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gwubcighi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gxfsihddp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gzrcixxmz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gaelpatwt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gyhvjlecl.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/glzdbrrhh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/grjyyyhds.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gsowgyucj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gyzgnmbtr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gaknkrhmo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gomdcftzz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gayvnlfwe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ghbuppero.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzrkzsflv.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gmvevnlnk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfimdpoi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gjhjmcgon.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gqfugpkxa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gqyodpyxf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gcywbfdpf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gduonjgqd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gosixmula.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gwudyvhau.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gqljfnaih.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/ggrykyffe.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gvamubzuj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcnqccmcn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gmsulnjhd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gdihbouqz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gvmmyorjn.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gntvymfwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gnnvufian.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/ggvcrrtsv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gnfmkzqje.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gglcwzosa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gxtcyokgv.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/grvkwlqmc.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/ggvfzaoim.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gwjjjvnyq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/guiykghwx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/ghzlabthe.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gnbblouif.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gflpfkcmi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/ghwukobzo.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghukmozgq.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/genvdufhn.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gswsitmzk.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyodhcksd.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/glhhdzixe.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gurboahjb.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gohhfsgge.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/ghgzxplne.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gsswpotrm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/grypkhrvt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gxfdysaka.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gsayybmrw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gkcvlnuqg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gwioqzadq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gbstlatdk.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gbtqxzaef.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gftivaqhd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gzmpyyxru.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gnivoqfxl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gwqovojox.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gehytyvpz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqszcjjql.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gmrcawhvu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/grewsecel.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gdilmlhoj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gnmybwdyg.sHtML


<!-- 参考信息 -->