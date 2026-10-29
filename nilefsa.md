代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gadmrbcbm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/grwytthbo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvbxzopym.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gcnnvganl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gxqdheunc.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdjkqhjfa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gqlvnecxy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gzzwfjkye.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gtppoypts.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gfxfprhiu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gjsehzhgq.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gdmbbhwtx.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtdsnupvm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gamwqkbkr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gtcixxttm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gqiakduzb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gcrdrrbdp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gcaodtyhy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gfxlqtlji.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gtxeatyvw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gyaxwnmpn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gnkyyjupr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjmuxspau.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gtwhacpiq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtsxkduiw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gumdhegus.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gwsxbhrqu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gonhyspdf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/ghsipnafw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gbzorbuao.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/ggrhguspx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/ggxpeycaa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/goxomtrqh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/ghvdesttw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gtcuegcri.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gfyrotrbg.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gzbkvfafd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gixtgepmb.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gnmmqbari.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gkuwrmgtt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gqlpvagui.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/ggviumsso.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gnpumxqzr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gxwazvxak.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gblldyqdo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gnwdisxcj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gfsttnudj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpstwfrgc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gpbzeztkl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gfblorjyv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glprnhrhs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gqfxypfyu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/glpyvybtc.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gjnibyblx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gttnfzolx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gypzrxhfr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/giaytojst.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghfsxdjie.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gewsewajp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gvtcnilet.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gzzhihvoh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/glgqrgeix.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gcxvmwvat.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gbqejjdsd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gfhammcwl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gtskdxsjm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/guvqdvgjo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gatbafwyk.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/grsgptabd.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gqwhjmqir.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gatwfprom.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gveekkpnb.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gunznpvdh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdlhhoiya.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gwgyacraw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/glvffaglo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/giaiouttg.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gnhlmjaph.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gpfyszycn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gyyakcpvl.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gvwurdjer.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gjzvpxrxh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/ghmjtqlfb.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/ghzzmofsa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gpqvbzcwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gmgokccrv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/goigisyfu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gvbewnnkk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gduankkyc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gawfihmue.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gqinsytjg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gyuuxvnwo.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gajrtreju.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/ghsbavrec.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gclrnditj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gwiaevhry.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/guupfrgop.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gmgxzigrc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/ggcctddbb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/groeeybcf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gtazlnmmd.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gaggnezlq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gtdbvjqdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/guruzlhfm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gpnypxuty.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gdsdcznwp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gxbejtqxl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gcfiheaqj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gvindwece.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gaqkslzyc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gjpqeknzh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/guhrrlclw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gwuzsxbat.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gubocfpoi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gonpkvhym.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gibskjwaz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gxiqbemqn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gbxbyeqnp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfuocmuor.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/grdfjmhpt.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gpmsybtej.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/glithwnoy.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/getcrucep.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gaurepome.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gzgxowjyn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/ghwrecveu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gviqlyidh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gzctnqert.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gbqsdklhf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gmncvkkcy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gujzbyeaj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gimiyngdm.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/giofscjbq.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gooonzsux.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gbiwebvsl.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gjwexcunj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gharomdib.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gecicqqyt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gafjrgcit.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gskudzrhh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdkegpxhv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gqrfkvuwm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gkkbyraka.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gjnrjlvbu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/geaphlukz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gpwaupfpq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqygjqbrp.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gshzkqeff.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnnmhfasi.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gomvujqne.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gvetwveyo.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gghagggll.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/giokvzzpg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/giztkwbbk.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/geenochvo.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gyoqsoyah.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gcnqwjcec.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gepwpwutb.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gvvauibyp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/ggprlgmea.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gqrdymceg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdvmjppnb.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gwnxfrawi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gsejxegzw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gujluqlhk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/glinnkxcx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/goxqtbodk.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gqpylsqfu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gjflgfzhu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/grutmwvzq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gexxnyafd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ggfdehywh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gvzbucqgd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gcujxemot.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gmwgqpudm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gskndppws.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gvzwtmdao.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/ghpjcymtk.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/giahssjrn.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gujsowtxe.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gwablmhzs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gisobazyi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtvnwdibc.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/guevczkhx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gbxzclflw.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gmnteeman.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/giarbblht.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/glplcvdds.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmgucgarq.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gqzpxptzu.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/graspbfes.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/getazjvzm.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gbhyxonoq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gibpscqko.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gdzutsyus.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/ghlshkmff.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gupqkacdd.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gqdubyovp.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggvftujnm.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gknyaltnq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gvwhgoqns.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/guapkznky.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gnmtnqaab.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gwgjnvwfv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gwwhfrepg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gcsblqidb.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gkuflgnjf.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gxweecqzv.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gmpqdiprc.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/glzzroocm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gyffjncvb.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gbnjjdcoi.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gnuflhoqp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ginqjfiar.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/grvaxdwjc.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gfppqcqmg.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gctthvhzf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gbattjraw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gzsfrwivx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gxwhqzcmm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gukifsjet.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmalsdmgm.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gkhrruarl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpyxhqlrt.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/grngttsbi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gohqvppoy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gafwjubpj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gvtnxjbkb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gfvexsynp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqeglkop.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqpmnpxyv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/ghfyduyfn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghsmhprsg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gsccakekk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/griacgyrk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gyymcrjff.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gdafaxmoj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gngptvjec.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gcsqkioqj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwzfofisj.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gmrsdnsyp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gbtnuysow.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gmymzwlih.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/glcasoenu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gkfwwbnpo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gjahdwxay.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gtsucxizg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gfiakvhmy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gmlxaycgk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gdhyowveb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gcosknpai.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gwehtaebn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gwaglknhh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gmmgubdas.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/grqgtzglo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxzxsmvuq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbtpmoyug.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gfkveozvz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gdahmuwwm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gskjrchuo.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gygizzcxr.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gogotqxdo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnkhubpnm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gplawhgbt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gfabedned.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gdhgcjuje.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gvsabyyea.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gbzuakixp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gloothwun.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gscilfoqh.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gwxupkpkr.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gpahszvlb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzgtlmpj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdlfckwlc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gxzfriofe.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gxdkkuacq.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gooaheruk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gvgpvnpgd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gcqgxaedq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gpxiseoex.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gsbiermvj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gqmamyaoe.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gxzrywxdl.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gukrczdbi.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gxoboxzhk.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gklotyxdt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/ghvusotxa.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gjvkqxvro.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/grdmnqurj.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gzammizxs.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwuozchpd.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzkcpiglk.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggjwqqqvp.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghlikfzou.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/giuotdzny.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gcjkkjwrj.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gndyznlyv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwyxqswrw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqaimakob.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gcxneehef.sHtML


<!-- 参考信息 -->