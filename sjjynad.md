代发 wailian999

TS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoulamhr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gspxxxofu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginztocmo.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmgmwink.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmlepgu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaegwyjk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggodgdadm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbvshlvt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjxtkjnw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grlpbwtim.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqnoxehn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghckrhiam.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyejttly.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbyiruki.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmachsjia.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawoqwzjs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fanxiaobao.xyz/Article/details/gmbffobmk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gqxenwznf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gmdfxnbbo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuwgppwg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtftromd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubyjftlc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglirbpzm.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/glvbhyzfv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmcndrcq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fanxiaobao.xyz/Article/details/gmrkqznjd.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyfphgvj.sHtML

TS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/giayuzsbe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gergdkooc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzepzcra.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkhcrglu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnmtbfhu.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgwdhtla.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/grsxfdxol.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdfwfheni.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gthyaugtg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/guesajfxs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gbiumukif.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gytyrmgac.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmibnsoun.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gooalvgba.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbanlixx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrlqwmxb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fanxiaobao.xyz/Article/details/gdvjnsfll.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gnvpokwrs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxthsfro.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/grflxmwhf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdjovmzv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvspvtgvq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvrvwgcl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/gocemoyfh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnfahfjn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuffejud.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttrpqrgu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/grmhicakb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbpnfxdi.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gndqdrmvs.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmfcmxud.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gmonhcrxd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gamnshskj.sHtML

L. 网络请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdzuoryl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gieazplyf.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxlfkqtr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfhokklc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmgdbidt.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrjebiou.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlqiyreq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwtgiruo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghucdgnwx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fanxiaobao.xyz/Article/details/gucqgpzel.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbxtzucf.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/glfiasxcp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/ggtlvrgza.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkzbkmjn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotbsesqh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiwuuvxh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/guzwrnebj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fanxiaobao.xyz/Article/details/gkbrpzgco.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvabvjssh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrsmirj.sHtML

[L03] 设置自定义请求头
来源：http://3g.fanxiaobao.xyz/Article/details/gmjbntqup.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioqpbxsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtwrzahs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gowjehurb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gqlemendw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fanxiaobao.xyz/Article/details/gefvhbqdj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvozmghwr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fanxiaobao.xyz/Article/details/gsnmlsrno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gtznvpuxf.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gazssejwe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjovyojlh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyallire.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gnnwbqfkn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/geoodowtf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/glvseljtq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/guupjovcw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyfzkqmo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwaqnsjm.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcptfehbj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gnfllkoje.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fanxiaobao.xyz/Article/details/girvesixp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtextzai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbaevafa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gfeosfdhp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqononpoa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfifvuztd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gkyolvunk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grkknjkym.sHtML

Py:   resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzvsyqje.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/ghtvdqmmq.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbntdcaii.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gualmhrgk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/glsprhxpn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrpnvrbc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gcmlbcjlv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzlpekok.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gdvuunsgg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqpcgxdc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gpewzlxvo.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/glwstovlx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gygdkavlg.sHtML

Java: resp.statusCode()
来源：http://blog.fanxiaobao.xyz/Article/details/gxfnxvzel.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gdetxqgph.sHtML

Ruby: resp.code.to_i
来源：http://baike.fanxiaobao.xyz/Article/details/gtvcuafdk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrztlesu.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/ghedoapxa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnovgtge.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaywngys.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/glaijfynz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gqoxxbudz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fanxiaobao.xyz/Article/details/guvophobo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtwdvhqb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gopkzmqyj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gckqgqpai.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqkkidaxx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gubzlsiae.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gocobsrsz.sHtML

[M01] 读取命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ginpgujes.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjpcqkun.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtxuribh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqjazixk.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gahbitvgf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgdoshsa.sHtML

Go:   os.Args[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyftevmn.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gyasvcrqm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrkhyjns.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdthbmwbd.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/goufkkwuy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmanblkz.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwmptkff.sHtML

TS:   process.env.HOME
来源：http://m.share.fanxiaobao.xyz/Article/details/gosobqywq.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gkadfajmr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gogppwlhw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqnsdywq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gzzswyzew.sHtML

[M03] 执行外部命令
来源：http://blog.fanxiaobao.xyz/Article/details/gnmpkkloe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsprjmoya.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fanxiaobao.xyz/Article/details/ggjxgozav.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gbclhuuou.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegbhvjqj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfhtwoya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjydpwiqf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fanxiaobao.xyz/Article/details/ggccwpisd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/grosqczdm.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/ghzzznjon.sHtML

Py:   os.getcwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gfkhuejdg.sHtML

PHP:  getcwd();
来源：http://m.share.fanxiaobao.xyz/Article/details/gajxueypg.sHtML

JS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gsqifmvid.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/ghodduvah.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwosiifi.sHtML

Go:   os.Getwd()
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjqxcqu.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gatazxaxw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/gmlxcteor.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gqbtsjobi.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtscyepji.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnsywdsj.sHtML

JS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxsksuea.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glotslsrz.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdedlvhvs.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcrzlqad.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/glrmhqplx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwiolxkq.sHtML

[M06] 向标准错误输出
来源：http://blog.fanxiaobao.xyz/Article/details/gyzyjtpaw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfpdgvjr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyawabni.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gxbzcqwmh.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/grwhvdvps.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlfxevzw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gpwrapnkm.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/gjolgyonz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gafzhfyby.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlonapnb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fanxiaobao.xyz/Article/details/gcvtptlzk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fanxiaobao.xyz/Article/details/godgbxjln.sHtML

JS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gnegoryel.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gzcozanuz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgxiihqj.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gpiaohwsq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gjagdpzez.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gthuotckc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gafaqgrxy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfldelaxx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqstqtzqm.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxiadyiz.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/grrplsece.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpeepgwi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvkatny.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxktekjen.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fanxiaobao.xyz/Article/details/geteiabfy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxuflyzad.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/gvvzdqwsh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvlbqqdsp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzfvhccp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcnacczhd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiuauqxb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnizvupqq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuolawjj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkngbtqun.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbernpxyl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/gccoynwmd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/geswcgaft.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzukddcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtubgyzz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpgsdnnpd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/guoobidjx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgobpfci.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gfuvwqiwb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxxaultm.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/geifvsjdr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznytlids.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsgktqte.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgqtkehj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fanxiaobao.xyz/Article/details/gppvlecno.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gpichiraq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gstjsmylh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fanxiaobao.xyz/Article/details/goeyugpht.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwximzdg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gilwxfyhf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdgocxxg.sHtML

[N04] 斐波那契数列
来源：http://blog.fanxiaobao.xyz/Article/details/gwqzrkdip.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gctewedur.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqdrplogy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvizumqpy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwynpjwg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcminobo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgksmoyv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwuweidn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gjzhbmrru.sHtML

[N05] 最大公约数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbomqwzpy.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhdibcca.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhkokzio.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdubkqtrw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkwroqpv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaebidbc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmecupviq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrowqlho.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqpmoikx.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gruhsfemc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghodwmpqg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvagrmop.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxzhshlb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtmhibzl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmhsxaco.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fanxiaobao.xyz/Article/details/glrscmybf.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gkimdgnra.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fanxiaobao.xyz/Article/details/ghtqoebbs.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gfhubiqrt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvqfrvyn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fanxiaobao.xyz/Article/details/gucjtfpmh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemnqnpwd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fanxiaobao.xyz/Article/details/gifaegkol.sHtML

Java: // 手写 HashMap
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfvbrkvb.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwmhyicl.sHtML

Ruby: // 手写 Hash
来源：http://wap.fanxiaobao.xyz/Article/details/gvgjzsmge.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/gxteawyhy.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnjnhais.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gglbxsojc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlatiypo.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/guzeusyjv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkssavav.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmujlasi.sHtML

Go:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gmffusgxw.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/ghzqkupzg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtglvqpbp.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gtakihktm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/giuzmxzdp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnosqqegu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzyvvxkt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fanxiaobao.xyz/Article/details/gxnxgbqbi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gouhtnxdb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gtflpgvcn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggepbsoec.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gznhvbhqs.sHtML

[N10] 链表节点定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcjtzruj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gwjpjcfee.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giiimfwca.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacxmbvaq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxckcrml.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwiunxcp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fanxiaobao.xyz/Article/details/glwncvuzh.sHtML


<!-- 参考信息 -->