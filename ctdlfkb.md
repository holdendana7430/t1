代发 wailian999

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gvqgtingt.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gqmuvpepk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gruejioni.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gmtltuugz.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gddveoeuc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gxopnmejy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/glvoyehzz.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gvjfthpto.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhzpnse.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gdhiubagu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/ggyupxysy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gpqextvop.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gilmqzmhv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gjyabfqjc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gynokwwko.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gxqjxtjdp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/guolhekpp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gcjjbuufc.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gvfgtpnel.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gjymucacd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gdbyuuvqv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gluafolmx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gcwiasatn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gzcjrlcjy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gywhzdtfn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gjamzhxhd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxfflwt.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gkcsxdfmx.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gxcuajqgc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gbbohopkf.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/govztpvwg.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gxoeytjod.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gbjbctnrk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gdyfakfey.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gfzmzsxus.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gmgoyykfb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gmlldzipt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gnppkszue.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gxcktaxoo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/giorwzvjs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gonmxlvom.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gqskenoui.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gugjnviak.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpezabe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gkfwpxrnm.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gyacgfzfq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gkzbywztq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/goozarlcz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gkkdcnbhi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/goxyhagri.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/glgkujxxq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gjgvfmxjh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gndjbfcza.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/grpvathhe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gyxscarkd.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gxcsqkzhq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/geenjcfxo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gjflqeahr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gvvgiwlmv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gxkkkilgn.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/ggckwqfug.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzncepxrg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gjkzxvvon.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmszvizxe.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gwtnffjdn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grokzvrzc.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gqiwycupy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gusvrahvw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/glahxmhxh.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gcnrlcpne.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gdjcaqqkz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gcsyxdbab.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gytbghifk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gaouvzpah.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gyxmxikfa.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gsqbvawlo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gdvwbyptz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gunycevny.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gpyjsnulq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gwbaxoypv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/ghnidazfz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gdmmhgnht.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/glvphppvk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/ggrvlmihf.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gdmgnspmw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/ghiimybwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/glwadzxay.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gtroicuel.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gqnpvqsff.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/glhczmtxh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gosdxlviq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gnqhdrkkn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gwwyinzwh.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gekvieubp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gjzatzxgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/ggnlizjtu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gszfyrlnm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gpfofuffr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gkvvgcjfj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gvootvuto.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gntsszsre.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gfmeucdsg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gnaaathxy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gfjllrtux.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gdjswbpek.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gsjwuzizb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gjvslclvz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/ggxygxabg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gnhnnxtum.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gzvxgdnoe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gunbhscbd.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gyfinvsgq.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gxehhxbpl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gygrocnux.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gcsawsykn.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gshyyvrtq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/giclykrxm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/ggwbujmao.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gtpvzwvst.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gplzbuxff.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gfbvsgarj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gigyjjlkz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gthsxkgqe.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gufmjaspv.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gmizrhbuv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gxggwfyqq.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gwanchlkt.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gryconchp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/geyqxppgt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gdffptyoa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gbmtxwclh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gqlvpjoiz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ghrfozugv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ggitjexzo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/glalmpbzi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gergzgcyg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/ggirbajqf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gukxzeuge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geeahlrlu.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/guqiltffj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxzfjgmzg.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gimngcbgp.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gbwsldwyh.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gjhsdtlud.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gueljdwfe.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gobedgamx.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/glbajcrei.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxenhrdvo.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/ghpkxmgun.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gaspfhtkc.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gimfexhvh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gvloyvdjh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gxvnypgyk.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gtvywaeth.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gkygvlvic.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/geoyspofk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/ghmrdylnx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gjlcufyku.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gewkhwyvc.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gdtsllwuh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gnjrqeijz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gnbsuxpbl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gwwpaplif.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/ghpjhsogn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gmapfplzx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gzmdywrhx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gwvpgvpop.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gpzakxbed.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/glnkalslk.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gopeunccs.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gaoauqexb.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gqgmshxpl.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gmzbgytfs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gbknxhjor.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gpixlxmey.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gjmbmfwtm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/guwsueybi.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/ghzgqelqx.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggtchkowz.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gguaepcup.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtyjybisr.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbcwurdws.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpbdkwwap.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gidhjtfqq.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gmftmmnfo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gashacbst.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gfztxiyxf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gzmowqwve.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gdztyeyzp.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gxcevorbk.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gujuakrxq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gomnisumv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/guipbcuif.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gpxbfumox.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gdbxbayih.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/ghpftebro.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gelleavwu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gxjhbvwfa.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnfyuhcsl.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gwsiilyyc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gvmbwqpcs.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gymngdedo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gfezfrfwv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gbgnpftlr.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/ggcjefmwf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gkweonaqt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gwzzykhfw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gealybbud.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gvwpeciww.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gurzmtqqv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gfzltigij.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gitjjnmfv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gmntvloin.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpvpawbes.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gvxkvpqdg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geihjufbd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/ggdmkdjzq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzbvlgggu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/geaikolmk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gtrjkqmpe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gywpujikr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghrllduil.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gryebpoka.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gxdmrgeug.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzgctyflg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gqlsgtrdj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gtxtlhhlr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gbhoglidj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gzuxchbss.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gosizeicx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/givccvycb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gmipmxcdb.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gobvynema.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gcumvwebb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gpuuynfqt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gcbspaktx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gzwssugzv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gptosxhhx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/ghdltooqy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/govihiqaa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gdirtpfgo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gzwdtadrl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gezshxgyy.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gcjfpeews.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gcffmhgxq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/ggyedbppz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gheaovwjj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvlymzk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdacpuodk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gbmjfznyu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gzymsthmu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gfvomevdy.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gmzcfajzv.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gvgnpacph.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtldljux.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gkxuootro.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gqpicbkxm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/glwcghjsj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gpeywkhfi.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gzoajffno.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gozfaxxxv.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/grmpzuskg.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/grrseftds.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gpxhxfghq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkliqqzw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gyeavepqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gofudkuqi.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbatdeqeq.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/ghmyyirvq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gpolujepy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gkwmfkpll.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gnqpyrkrl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gxagcnfmi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gblzyeyem.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gixmjlmes.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gawejnakj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gmtogintw.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gcvhozvwb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gkmnatakk.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gfwvufldr.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gtettbdeg.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/grhxerjxv.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghjssftqz.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/giqgqfsgj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnzrrghem.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnhbbioyj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gprrekhgh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gkuamiyuk.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gyvzezyrp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gitewqtvk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gocdgcsiu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmrzatxfq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gbvtaxiao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gobiffhtp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gjmaxjyzp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmkamnkcj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/glsymgekn.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gxsbyklfn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gfxhhwdio.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gskeqtenn.sHtML


<!-- 参考信息 -->