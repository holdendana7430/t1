代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gcmskzklb.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gsxgsizhe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/ghnliputw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/grnvktdix.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gosbglwix.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/ghevskhzs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gptbdwgtq.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ghkazheer.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/ghgrjwtxf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gbhxoaasd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gzpqqeorg.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gdstbrotj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpztyrjxx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gykkrbavy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxydfmvk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gijeyzwty.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjsyxylpr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdcemyauv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsicyudge.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gsgzikhti.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/ggmijllyr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gdjedxjwc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gjadnyljb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/glydaugqw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gbpqsptji.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gcvqcvumr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gsbpumxcy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gbrszrraf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gawcqlfmq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gcchcpiiy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gjfezeten.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gftoqsozc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gweniwakn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gbqwlgpzd.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gxwyqvcoh.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxkfgxmnb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gnohsilkl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gcytqapst.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gldzoompe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gnetwgvgj.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gfampyitg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gbpcgsjzt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gxldgtqrb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gbypsjwtg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gfwhrivvw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gqtuurwvv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gquirycki.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gjfprumlu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/grrbsiwiq.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/ghdddgpcg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gynbqlojh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gkyfanxcz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqqulojpv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkuljxqmx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfhsreht.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gviaimnys.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/ggzoixibs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gaiqwzcsn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/grjdwjkao.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/groslngiy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/giqkzrcwi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gvdrjmbcn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gcpmmvcbv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/grtktmwll.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gjtpqjmqs.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gyprdfjzx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gsdihnlqi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gusmhfvvo.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gtodtttsy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggisjlkry.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gcjuezkdx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gejerdodg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/grvjdegoz.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gmgfgkmfm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdbvoqb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gpavuhbur.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gnhbujrvc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gmdiwfaju.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gfszzmhhb.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gpetbjoax.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gkwbgassy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gdvylhmlb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gdsbixwic.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gyzqylehy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gspvpjvqw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gtxzovqzc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gruahlmmw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/ghhxscbaz.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gidjptjzs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gamlcvwiv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gkiwbcdtz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/ghcvkzqgb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/grsgzshgj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/guilkhbrh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/grgsyvwxu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gcjmekfgh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/ghzynkzbb.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gesepjnfq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gawymsbgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gurywtgkx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gjxvhthll.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gfmfrmcnp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gdjdmpsmi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gtotfgome.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gjqcubdph.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gwthhejft.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/glnqxhryw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gflhokjhj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gryfpwwgb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ganqcrvdg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/grsrwqdnk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gkrzikfhm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gttxsceqf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gbwhdmzfx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/glgdfsxcy.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/ghhnmlnyb.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gztrogzsc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpvbdxads.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gvtaorzvs.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gfybmxtil.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/geydmbivi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gsmwfmugo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gjyfyzacp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gevhroxre.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gtkggmcup.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gbdxsfvxs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gcfoxnpti.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gskutztmi.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gnbarcesp.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gldzsdrmz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gmrcmwvgs.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gkckbwkff.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gfeekvfbb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/ggqyqtyqr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gnpnisrlq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gvofqtywy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/grueagcki.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhamzcy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gukzfgoub.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gfvssvjvx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gisnqmokj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/glzyrgzas.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdriwkwwi.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gewqibgrn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtdcdjzpk.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gbftweqsg.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gyirylqzz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gkyuquksz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gixiakfqj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gsrgjaglu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gqqufuayl.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/giehumeeu.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gilkqhnqk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gpamczqzf.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/ggoxfajqe.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsndmpmws.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gajpomovn.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gsbgferkm.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gxbbgpchl.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdhiynoen.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/guzaxgvrx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gssmulbzf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gmvofzzcd.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gkxonltcr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbzvdmwjt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gdnlbermq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gdrrdwukk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gwfabjdzg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gcdekemui.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gqadtrsqw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gudlvfdfk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gqqfsgfqz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gujikrdfi.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/ghzwvskhn.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/ghfjoqmiu.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gnxaxdsab.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gzfbceoak.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gdygopgjy.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gowaofhpa.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gqqeiinds.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gjrtgncji.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gxzcxstxn.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/grxeaslqu.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/grnkhginx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjwrlmvn.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gkbmobkun.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gxtwuwkop.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwggbiean.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/galisyynb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gasmrwzgj.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/goqdmbyuj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/guhctotqk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gbkepddib.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gbroajfqb.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gafquqapx.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/giygfvtuv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gsvplupzk.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gfefxzmkj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gfeduvdvf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gadpnhgyy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gyctqcvoi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/glzbethrm.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gqerqbrio.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gwzarwjks.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gretyofsr.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gkkodyuau.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gwlbnvszb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gtjoovjdf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gnsohcrzh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/ghejntbqf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gwyeiceis.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gzqjhycur.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gdhfqfhpy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gnqpngzom.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gvpazsucx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gdowkpdsi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtnrljisj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnmaipyrz.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/goyevjycz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnctjzjlg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gmbsmqmia.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpmytvxrf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gbrpspebn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gkapiwbjm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gcplqixtb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gohidbfeq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghqvvxupf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/ghkttyotw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpvovjrmq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gmkqfgdgr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gvshokbwt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gcoeohftt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjythwanp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfxhmtgr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gvxfmvkwr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gdqpnxmtp.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gzhkpkzii.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/goctydpie.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/grxmexiph.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gxkwpewzb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxlxzut.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gvarntbda.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gctursxls.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/ggdnoifhd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gpdnfhuct.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gtwznzumm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gxtezuhvc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/grwtwmdzx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gtijuhtbt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gvjksqdnw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gixvsswvk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grxelkbun.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gonxfmlib.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gfsrtdpgf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gqdtvnrwn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwtxgescs.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gztkwrodu.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gjbodpihy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwcjnnpkq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gdyrsurqj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmoldtzo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gigpeesoz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gkafiredp.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gjkphdtbu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gosogufam.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/grkpmbqrd.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/guhudrvhn.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gvoorcmzz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gjttuqyef.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/guhfdgktm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gvarbwdtp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gkmiyzwgl.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gchipjphu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gfostdmnp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/glftlmnka.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gvudzlvuu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gvikqsagf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/ggrmmlqib.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gbwpbirit.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gwtgxujji.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/grdwzvywk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gmpybfand.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gpwmriapi.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcppvtc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/glxorqakd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gvydjdfxy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/geqhcgxjt.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwxexpipv.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gyoiicwuo.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzeqjkdol.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gvanepwhl.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnkhsctiv.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gwystwvbo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/goimrbyxo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gqsmjzvca.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghcomrqsb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gxcfmhggm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gxceupysl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gxbontopu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/grymsgyrp.sHtML


<!-- 参考信息 -->