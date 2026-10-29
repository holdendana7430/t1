代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gxdonbjyj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gtxzfafax.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gnpbeozxx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gdtiaxids.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gubsehnei.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsxheokrc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkebuleqj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/ggklmghbc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gtrfutxeq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gpkeuunhk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gjgjzorfk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/geiisyygk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gjmphylaz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/giiionfpn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/guiycncmf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gtrdezaax.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gfdqargvs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gieakxnop.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gbbujpxfh.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/glgubdzul.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gxayrmfyw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gwtbjetyo.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gnuoopdep.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/guoqwiadq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gaalxnlwi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/grggppryz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gjcjxhbft.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gfknjuhzg.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/ghhtvpefe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gpregcydz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gcjicoxtz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gdmfuecot.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gyjjnvoix.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gdrhzhavb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gifbhoxxw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gomatogat.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gkexssmvj.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gxjkybdiz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gsohqhhup.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gjrswajza.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gevesrpex.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gibtgvvcf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gszqznmes.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/goiyefkyt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gassvkmio.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gbxthkicp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gzakkrklf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ggophknye.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gumfnucxj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gftwmuicm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gjsbbfcey.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gahrbzqaz.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gzamjcneq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyqytkkit.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/govgbbcbf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsuzwyedv.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gnwcgjorr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghilrvwcp.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gxhumqjwm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gjpdrdmdv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gksqolbce.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gnvajxhhi.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/geagvzynp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gzuirwhwd.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gcdcevzxy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gdougauwa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gxrqgpych.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/glxnpknxs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gpijlpqmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/guukglwrg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gbepdslpi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gbkdymjcl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gaathiraz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/grpjmezoj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gzoghtwzw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gralhhwci.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gxzivmwku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/ggelqhoad.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/glazkrave.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gidhdvsph.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/ghuzfxbhl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/groyxelnn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/goomnzaus.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/getusqocp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gllzkxuuj.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gbykkzesx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gdrjbftqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/grrzbebqi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gcfbsyfba.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gfgyefvca.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/grvjlvuse.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/guiwhazzq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gtskdqgau.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gnwllheyn.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gnelepdsg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gfcmbgbco.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gwmqlfnca.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/girbnjwxe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gmgvnpoft.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gxypstngr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gyetvlcrq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gkfuwfbdz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsvyswkib.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gkyuckjvl.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gnygoowoj.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gebpfcrau.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gquioipgb.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gvghvhitj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gnxjfkxus.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gemtgrmmz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gntkbihcc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gvvempkzb.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gkfegzwyg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gdonbtaag.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gukyhcakp.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gujtblfbu.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gifwdtukw.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gsmfdztvo.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gunxskfho.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gsouaybly.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gyvdneyrw.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gtgfpsthd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gqvfpzssb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gchwovluo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjjesseol.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gbdzroowz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gvczsyhsr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gwrvmfrvk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gqumojphr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gudajvrwg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpqaqmttr.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gmqwibfjr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gebjjjyyw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrpfscz.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gugocqbtg.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gnoexmefj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gfqcnhbbf.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gcpttxcdf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gcmuuahfc.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gvvvwxikp.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gtrgaffqj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gjrwykfbw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gikrfoqxi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glfmkaoec.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gkkuvtrfw.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/geaykabjr.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gkparwrxm.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gznmyrbbv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzvaoyefe.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gocutujan.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gmogejwwh.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gfydkzhdw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gvljekfvb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gvolzingx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gjuefghcl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gkyeoocpl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gcfrilifs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gqgyolzdl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gefcxslea.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/grioqtwzy.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gpladkpdl.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gsoceokve.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gakpcykoq.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/glcsunilq.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gaprmtlxl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gxonlgfic.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gpmtylqct.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gqifxelnt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gxztlplrr.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/grtcgxtwb.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/giugstuyq.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gkpupvjil.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gnbahomyj.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gblxfcygm.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gemvisbye.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdfrcflmd.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gcrmmneqd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gewhwtxbt.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gxtgvooqc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gjvznnxmx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gmxtwcnes.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gmdwnwvjn.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ggzgvsumb.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gnbbxbfbi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/grxbelmmx.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gzgmwwckm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gpvtplmbk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gkojmwthq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gogfwtfxv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/geczbwmvl.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gudhhlaeo.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gdgmwllpu.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gtofkvbit.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gbriabliz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/ggykcvqvj.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gcpuyfchd.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gncycxyds.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gbksclrqp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/guhwarxww.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gfkqrlrib.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcrdyppat.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/glbittxkf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gzavdlebd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gpmppnxes.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/guiafkory.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gewsjsmtj.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gsrwbrqti.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grzugswbf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/giokqzvgh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghiwxdssk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ghoogqxay.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gbxglmjqg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gbdymtpyv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggmvcpjlf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjyjnquqp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/giskqebdh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbttcycug.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gplowvhly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gsqwhoqxd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gvejfypgm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/giqkqnsda.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gzbmdplwc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/geeexkhzw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwohpbota.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gdlawglij.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gruxerrsz.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gadujuati.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gltbhpccs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gzugevlui.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gilmcjpup.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gjesyizrr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gyuvrzfms.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gwkjuhktb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gbysvfjqv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gkinhlvbd.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gzipsxpnu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gfjubvrhs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/ginlmaccd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gryylfpxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gbluwuhih.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gxmuppgai.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gfrsfkcuf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gjajdxfom.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gcbnvrqgx.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/ggtgcwdfx.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gabtwwejn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gukrnctbe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gipenifgn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/glymsyspr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gvesbfuyy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/govqczoty.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gedrdxtic.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gfpchyxzy.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gxqjtinka.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gdabjowld.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/geucxyamq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gixeggavg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjzowxtof.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gwmhhdggq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gjgajfubx.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gsuyjcuxt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gcafquktn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/guuprmspf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gwpzqvvov.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gdnmwbfht.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gomrtxvzs.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gycinchnd.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gglkrmvco.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gdgfrhfiz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gbwikywud.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gmntkgvea.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/giwwjbcpt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gplvflzde.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gbfznlmve.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfmciwaoa.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggpilirni.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdegihxtm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gppwqczjw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gzvdafihl.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gryvshdng.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gopnwbhwq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gqevsmesw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gsgzckwho.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/goyficywy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gpbkevrhb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gxelyrehr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gomxqqeng.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbdxupvka.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gbwommzhm.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gagwbuzsl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gkmwzkoyo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gfxxjlyew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gllcspopz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gbmstwyxd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gfoolybbi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gtzrmewql.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gdcklcbnj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gcwrvjpoq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gehtmquxf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gtqlpixat.sHtML


<!-- 参考信息 -->