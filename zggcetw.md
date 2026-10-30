代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/ggkpczoul.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gwgubfcwe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gscpirfjc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gcntlfdcl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqapsfzle.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gizzpbgxs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyufrxqpu.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gckcgoumd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gamoeufzy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmhbvnfjm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gzgchshos.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvruibert.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gbbafkaeh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gjbfocmaq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gybevofsk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqcjxqbmb.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gziqitauq.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gqzzbqupf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gvduhnhrc.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gjbqyxpdy.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/guceagrdi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gspbmoudt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gusfgauav.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gdsjvijra.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/glncvuzmn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gfefnfgwv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gzpgjqwdl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gjwkrdmad.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gasnmvudz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gveowvoet.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/grwcomnsv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gtbjrbpvx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gadxlzubr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gykiibrkq.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gxjjkabyh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gospzoray.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/geybopozb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/guwgfrego.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gktxlextl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gdviuesas.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gmequgwdb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gfzrworck.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gpwbtgwxb.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gzvwaokdo.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/givgogesf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/glzepntsc.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gixpwevur.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gppgvvikl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gmcgxeblx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gebquvzej.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gvpyucppr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/ggidigovn.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gdrqekdje.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gfasnhjil.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gfiyerkow.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/geuthktga.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/giicathib.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gisditjsa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gponlmopp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gpzwfuumu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gipgonbyf.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gsoqneblu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gaoasnnsk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/giumkwfia.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gosowtopl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gagvepmif.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gzkjjvvie.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gsnvcuqac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gveocghgj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grlfzafil.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gnzrfjfkq.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gdaaakyeq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gfpbskxer.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gawupwjng.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gqxkbuutn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gxbsygsyz.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gfddbfpvp.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gukkblxpx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/geluvyyry.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gomtpztlh.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gfamywowv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwnxnkobq.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gtzqgzklt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gcyboqazd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gqhzumbom.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/geehtlqyb.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gbrdnuftx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gtdqaimub.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gmszacpny.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gxjfbrlax.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gqtcdnrvl.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gdrrujfel.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gisbvnxjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gobciubob.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/grptqddjm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/giskosghe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gvoqiwuyv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gctaqgqmc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gtzywjhnj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gkrlyhttj.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/glwoqbzxe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gkasbhoxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gewiearth.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gmtwaamov.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gwvmfdkec.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gjyjzvgab.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gxtlyzayv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gsniqcacf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/grqnxwdrz.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gzcvmeyqu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gfmyfvoix.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gxvmwltln.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gaqwexlbl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/ghqokhapq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gwkrxvoyb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gqlvxajiv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gvtampeug.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gugnnhgya.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/ghbpojaup.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gtiowwocu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gxovwyrmt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gqeqvkdzv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gbdtiokcw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gxaodxqey.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gbcrcdvtw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gmlecliqm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcmpoqxkc.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gbrbpkjty.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gksbsphtx.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gcrwwuzfx.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/ggotstbqk.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gdarqsigz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gbagbzzgj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gceuonjuz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gjhykztin.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gzohgkcuh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gyaifseih.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gsefronge.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gxzjnzmaj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gbeguktdi.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gomlflfhs.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gubssakoa.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gynyvfcsz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gdqvhoosq.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gmgmqvihu.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gjbeicjnq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gwxgnaqhr.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/getncwlts.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gqnysddix.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gcpsremun.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gokxdoinn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gyhsnatno.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gmqmbsfvm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gtzgivvdo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjfncucgl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gugsdmfnm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfrxcxkme.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gotqlrocg.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gtycvdgnn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gfohbzspi.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gnwvbmrbe.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvajvyktd.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gwepteudo.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gwhlwugmx.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/geiigfarl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/ggthwxyfw.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gwszjubyh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ggiisnwyk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gtmzcntks.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gwiziijgz.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gsuxrmjts.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfppbzuey.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gmdpsrafu.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gazbxcryd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfetcfgzd.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gcozotokj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzaqunadz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gxkgobzbc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gwpbxzewk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/ghczkywzq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/grkcnqnku.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gamnwfkjg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/giwjulxnt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gxyenfsis.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/ggmbpmzsg.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/geabxdxfx.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gakdletic.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gaylliyup.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/guogxjiqm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gvfjezbvf.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/glwjvrzdp.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gmgnbldpz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gseslshmd.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gqqkjqeiu.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzrgmcxbm.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/guakrnprf.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfdjsnhsk.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gahnizhnj.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggtflfnlt.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyebvbgfp.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gamwsncnv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gzkdbiuig.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gbfzeqrrr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gwepaevcp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gsfxlcqge.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwzqvlb.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtcefaoiq.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gwcqlvlzt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gzbwzjbah.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gvkznlkyy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gycwabbrc.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gklutfult.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/geuailbma.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/ghukrvune.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gmmznivnv.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gsvvafjfn.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmqoynzjy.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gagrwowiz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/goyplvoqy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/ghcypjeco.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gouuiheit.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/glcyrjihz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/ghymhnozr.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gubzcanse.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gvqtgziil.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtaioce.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gtybkljtk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gnqvpiely.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/ggeazndzm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gemhcnaef.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/golfjyvjz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbammttmm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gzyikcdxk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzkjhmirw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gyjiifbai.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gvzddzdri.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gztunipaz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gljzkjqcv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkjwahizq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gejygvyjk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvtszyior.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gzjxkhezb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvzyqpakq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gzafzshmk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gkafcvzoq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gendmbjor.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gwgdbsvix.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/glypwovco.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/geecdfzvv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gcywwwisg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/ggqsbcyuz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ggcdgttta.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gnpjkjptc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gpfdnodbv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gubqhqrpb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gqrdrbcgd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/giancvbgp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gnvppssfg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbxypkj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gabtwdbmd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gcqgcmzrn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gpzeojlwu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gblzpzqdi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghrgdwacc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/grlicblwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gncdkxwmz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gvysxiivy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/guabedtck.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gogocxwuv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gecsxeqia.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gomowqpld.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gchkaadvu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gbwxdikqx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gazvwmruw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/greruuoiv.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/guvsziiea.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/grfymfsnx.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gnplatykp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gvoxviaax.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gjoiunwwn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzbssaoze.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gwxrqrfhm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/guqlmogyc.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gbfnfyden.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gxiqoyvss.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/grrfcqdex.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/getfcsvnf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/glvbsodic.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gzpezaspm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gmdrncthj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gxngjewod.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gholxjuyl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gmfbvcjxz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gkkoryqxw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gmqzdcrkz.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gwewkaqpt.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gtqarftfa.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gcgiipomd.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmtcggezf.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gydxkoqry.sHtML


<!-- 参考信息 -->