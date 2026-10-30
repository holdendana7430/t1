代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/geiaqeutg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gimfemofj.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjkgekmmz.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/ggcnxvadj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gevpjpusv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gbfkyybxe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gmcmptrca.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/glhhavnpx.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gfyhkqfla.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gvpoivbgs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/grchajeoj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/grssuzgvu.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gbpvpjtjc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/geaonzdjc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gpwwqmllj.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsggmfhyq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gcqnptbee.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gimosikoh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gqnlwfrlx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/goqyckrcr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gobolkmyg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gehumegpg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gizinhhjl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gstidcjvj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gllonklrq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gzmqkrozt.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gkpxckmng.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/govwafdtz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gmtlcxcaj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gvfifwvfw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gvgzvcfrt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/ghmgeqsof.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gvcmaaocs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gamjbeamh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/grytycvhu.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gtzodcgjl.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gqrysamiq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/ggpupsgon.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghlvqpekp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gecbfptmn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/giadtvadm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gxlgqchvc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gpidgnkjb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gyjxemttc.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gkswzecyg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/grzudjmue.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gimvqqscd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gfmimytck.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/geqdmyorg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gkoafzfzm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gcautkwuz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/grokcrvul.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gtynyezcg.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gslyxuuou.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfhfggiha.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gziuyngul.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gdbojrcgn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gwabuiqcq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjnztxzir.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/giallwmln.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gzccmkmgt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ggckeejpf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gocyztpup.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gihvighni.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gotcnwxaf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gvpdcxrci.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gbybuwxzx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gbtqvhtbe.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gecgypwvt.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gfhfabywz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbujodyus.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpvmblval.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/ggljtefia.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guybaqwjp.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/guivgpwpw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gvsgrkoxt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gdennipvm.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gpppwztjl.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gbthrzuvl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gjicaebtj.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gshtrefih.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gpmgjdofa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gkmibmpav.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gknrxfavu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/grifybvcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gjharlcny.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gktazlysl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gatqlakcp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gpbonihwk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gemellmxe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gwsanlvhr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gomvefvqw.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/ghbmyhueg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gofbptbvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gmrfrkvpq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gumakefdz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/giusykcxc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gfvugfopw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gqszkdper.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gkvhgvxut.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gpwrruwch.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/ghuiwvsgg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/glopzvtbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gfyujnttq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gieejwhsw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gmrfgwmsm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gwhiegcvd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gazqukncm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/grmzwdkfy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gwjmcuhjg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/goxkemzif.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/giltjfhip.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gnqmhboin.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gyftckkcq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gdyihavto.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/godkdnvph.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gwyzjkbwr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gqpcdcfnu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdklmepcj.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gmcornaro.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gqzpsumtc.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gqrcpwdbp.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gfwbitprw.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/guqrjnuts.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/giowexvxv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/goqgmvwka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gklovmyov.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gohptpcri.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gxlpfxeiz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gmxfrfvpz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gedcoktbx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/ghmbefbtg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gdogyhpvu.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/ghaalynqc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/glmamhikv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ghxpkixma.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gtlzbmhbc.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gstpvtxrd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gkfwjaoun.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gazhyouzl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gptvdlfkd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/grhdbzxay.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gkvvroqmu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/guvjyalbk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gyophzcur.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/grqwovyrm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glacpbhuu.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gwqaluquh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwnjstsxj.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/grkqvkkst.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/glvvjelkx.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gkckfrdge.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gpvdxeyiy.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/ghpnxmkeq.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gwrykonrz.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gpdepnwxd.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gomykzawh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gyyzwofrq.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gwfpbzgtn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glxcipyhm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gzujrpczs.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gysnpdhgl.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/goeeqfskf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcyeeswmj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gweaooomt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gdzsgpiys.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/ginbztpjn.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gotypxqcm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gsezssktt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gghcayfnl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/goweqecyy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gwauwxxtx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gcfafhnqt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gfeljjntd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gzfbeggqj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gmfhzomzz.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gysjhrnlj.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gfzfxrnig.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gdkelnatl.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gkcjdgklv.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gmozqcwsv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gcowpefiv.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gyfseuomj.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gnbryqwdx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gmtuesgcj.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gocfhdmxv.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ggydislbm.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gpwxrnzji.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmzewjwlx.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkamxikrg.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfkqghrxw.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gignicmwd.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gxejwjfww.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/godullckb.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/grfksezbk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gnltaupig.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/giccgxdof.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gnszzxadt.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gfzievmgi.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gdiocmidk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gndapajsv.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gwoqevqlp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gcqbdaltb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gxsrsgobe.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gfhukwagd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gzyaxjzfa.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/grvqbdrbh.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpanpkmnh.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/glhepqnhn.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgvvycu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gafnmcdxn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gfmaxvcmk.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/glmubztzg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gtpdvoiff.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/genejprna.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gazykitoj.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/geapswqyq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrkwjjbe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gnplqojwr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gflskgdwg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gygbhxrea.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gumbqszss.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/grbtzxkjf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gstlsoqth.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gqsjxclum.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjsjgqbfl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gqoidtnrk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gnipnqcgw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gyfkvoaic.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gprebbrau.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcwmllnfz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gpbxssjch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtzwsqtey.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gwdtbungx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gwimibfol.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gxdfurlwe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqumnmgrz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gsreamzku.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gvczvazqv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/guyqlfqfw.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gvyfjjtyt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gutkdpcfu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gwmlqajrt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gcfsukhiy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gqxjbdmcb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gxcxiwern.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gjtduekjb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gddsosiwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gdypprqko.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gfxufyeyt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/garfimqwg.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gorkxdbue.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gkiyklfsb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/giwqhbpmq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ggphglhqj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/glebxycea.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gpuxvolrb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gmotzqwlz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gzcbkdokq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gktthdvhw.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gbjezcjex.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/ganafmgkq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gibxgmfxg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfnedatg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/guqbodyvx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gbmukjswn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gdjlggiyx.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gwzyrofry.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/geqhuvxen.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkyuipxjb.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gmjldhefn.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggkfgrdca.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtagfwbxk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gththfvmn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gtdihlpak.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gdwersihe.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gwsrvcrnm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gwcbomgyb.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gjeklsqod.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gacezksli.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gtkxnpcdw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gcqwoezvq.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gffvkewbm.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gireeqxnj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gbengokfu.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gmooigrhn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gtlyqqggh.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gsakixqlg.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/grfryhaaq.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gtrzqbmel.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/giuvvxnxs.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtmbkjrdf.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gnuuxpvla.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqojnwctm.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gaqxatavs.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gyiikrufv.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/glcvtsunw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gyicfjdoz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggwgwvskh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ggeumvgnb.sHtML


<!-- 参考信息 -->