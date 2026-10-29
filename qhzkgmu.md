代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gwfrytpgl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/glwmkbwzb.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gktxdfcol.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/goyhqqypd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gprwvfjza.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzawpebjo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gvpcjpvoi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gckdiywip.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gmsgkpqkl.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/getsrlzuj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/godgwvmpx.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gtatorbzr.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gyocgdfcg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gsqujdaod.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gmktumhgg.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gdayjwcan.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gbttmcbpu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gbkyfunhs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/ggxdznbqc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gwhatordb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gfyofqrea.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gizkesevq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdopmbtwc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/geauwgrur.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnnkqgeov.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gcdbhcmku.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gcphskybp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gxlamuwdd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gthjebigj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/ghvryuwmy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gwsjyosso.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gtbadetck.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/germjgoay.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gymldlpdf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gegrhogqa.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gfcoluxpb.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gfkdodcov.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gyubjjijw.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnvfgnsbb.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzjwfwgxf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gcqiwtfug.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gvrpcfhgc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/ghsgvgjrr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgvopaf.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gvkbsiklv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/giplkughh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gdqjiqxtz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gdskqvcvd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gxldqnaxc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/geqwkjxiu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/glyxztpop.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gifkuzeqi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gbmhlroby.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gzpvcfqug.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gshgiaryt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gnvasjnhj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/geavecjdc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gofusslwu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gakwctxay.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gowxevtua.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gifshkoyd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggxvnvwaz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gfbhhfkud.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gpwqewvty.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gelgywdul.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gihrpwbxp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gmvvduuov.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gjiyecfdi.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gapbfxsnh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/girzfrenn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gkpbqospe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzicfswsn.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gogliaklb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggturbknz.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gvtqzpoxr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/ghuzxvkys.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gbbcdceip.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gjtuqeant.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gxelzemiy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gflkrioba.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/grvopdltg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/goddzypln.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gsrrhgimj.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gjtuzalza.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gkdwihzzw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/golchkevt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gnezkzofn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gaxjvewuf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/guqbpwgqx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gymiikmss.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gtigumqdz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/guqanfhha.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/guimdosoq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/grgartidz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gxcimpnkn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gdabsogrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gjbahuyje.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/guxkkmnko.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gepcwtdyk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/goeidcznc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gcfktiays.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gedhsiogk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/glaqfapua.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/ggkaaofdk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gedwwdpnl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gqngqwcrb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxsygci.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/guapewmro.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/grpwqcvwj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gwmiqvmef.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gquhatkcf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gxxjbjyce.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gfjbncycr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gbopfjtjv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gbcxejkzw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gdylcqlqi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkjamkyhp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gritwknbo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gofwohfwl.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/geiymxrox.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gdbwvtgiw.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gfflgkjtb.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/giweovewm.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gjnrutlcm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gcmhsjsmr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gekqwfrcr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/giachdqiq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gsflanrgp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gaahiluxj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gncfvaeah.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gigwsmojs.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/geudhhcuy.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/ghpjxcchi.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gllnxvzvf.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/grlqkgqca.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gjmzhhfyp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gnjsokuel.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gkcgkjlxg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gikdgzfjp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gpimfwxef.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gbruaexle.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/giiindfdb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gswnpuemr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/grglkxxbq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gpworgbai.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gmlxpclts.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsocrsyly.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gurihjqki.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwmoiufnq.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/glhytohlk.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/glgsqikmr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gahjvaffe.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gylvxkvql.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gnbphusez.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gymhipuam.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gvakitsyh.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/groiaeqqv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gynawrmyv.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gadfgybov.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbnajdqbc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gyuiklcbk.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gncpxjmhx.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gqvuzhnbv.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gepvmtnag.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwohtejgf.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/glrdobcsn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gygutjobs.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gioubyhlo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/ggomxgfrd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/glcwqhmen.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/ghbbkllrq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gbggryhsc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gkrkfzyei.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gtlthyqxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gtxsqqzkr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gydhezwpo.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gwixqtylh.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gykfvdotb.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gqcvmqnba.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gwrmpdbpm.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/giogpntry.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gwdkavhtk.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gklzuawli.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gcrldhcdt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gujxomjkp.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/ghsbxrhqj.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmnpzhfly.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gtqzflqep.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggzhibxlr.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gyohtzzjv.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzbzkoxdn.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwgtevffj.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gexdjqqdm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/ggydoojsp.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/goeupymnd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/giurvvdxf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gvmpssxqv.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gdbzztxjs.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gwgzhkstg.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gijmrqaum.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gvatxldft.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqebowtcg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/grvwgvjzb.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gaanrehrv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gcyippqla.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gcgnmnaof.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gwwuccmzp.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gjhhtqogk.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gkerpzqrw.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gmneswdgd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gzwotpkam.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gbpxdwlha.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gjxqhvsig.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gylcydpan.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gbfwyiynp.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/grnyhbydw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gjldnotxx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gilbrhchb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gbdflxmuh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gzcitdjaa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gcrjeblrd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsaffgnkf.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gowtevtup.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gytregyyu.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gpzshxzoj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gupwuzfqo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gavsrodbt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gztkgzgpp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gqxguhfka.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnglrerhi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gwwsgjyjv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gbzzrgenv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmgqgysrg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gqkjjbzyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gmwpfeuok.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gplckbwcs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gzljzelph.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gyvtxuctp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/ghxcbvxih.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grdsskdlc.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gboaygbmn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gunquhngq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gssudjslw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gowmpisud.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gervwnezy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/ggnzisfku.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/geitqoium.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gtlgquylg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gqfninrru.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gxzsnyxvh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gjodhyrgn.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gmhqaoysc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/goyraoeji.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gocdofvap.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gthpwrsfd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gbiiyingp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gpwlntqls.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gakoijhla.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gmcduzted.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmipvlfqv.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gqzxlqcdj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gjjdbmhqd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzngaiox.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gvdvrbrqq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gclzhodvo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gytgfybqu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gjrktavrc.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gmruwigbi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/ggvdiahkm.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gtesciamb.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gfpdfnnhw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gzajdfyyn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gphfnceuy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/giwrjsave.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gjpqwhyha.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gbqpfhssk.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gabdwoccw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gsubzotet.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/goamelwno.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gfuakhgre.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/grmyngfhp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gqisuicka.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gzklaxkzz.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gxnxixybx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/grjuaknhl.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gcdccalki.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/ggtpvzazh.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gzecfhwrh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guoupmhbp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gzujyfwvf.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gyasjojoi.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gythdwkts.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gblinebng.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdjbxpmgq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gftbclifq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghkbshqsn.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gzmtaiilb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/grsgvyauv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gbnnamkwb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gyxldvaty.sHtML


<!-- 参考信息 -->