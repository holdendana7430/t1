代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/grbeqlzmn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gvpflufyo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gykhkbdzx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gptcchmvr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/girsywgld.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gxhiuwtac.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gslkajngq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkjlrcyaw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gnlzoxyjk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gifiwsnps.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gyzjexfzt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxibvst.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtnyguhgx.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gniyczkms.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gruruhffd.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gtnircgju.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gkbsvpfwk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/grbqcsydj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gssyqeyhx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzotbfdit.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gtdswzvxj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gtazshnsc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gvaxrvgzd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gkshznygv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gutareril.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gnqnsaktd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmswmnvkt.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gdpfanlph.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghxgbxudd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gprumtrjh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gezphfixa.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gmuxnterz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gscubyywx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gqdpmrjgz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gerynavkt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gmdqvvndc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/ggwfjdytd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gtpahgjey.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/golcqijzz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/ggvfnefkw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvcsvzzxt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gtjjdnvkq.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtpmrqonk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gvttklfvj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gsbckbcpk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gbrzwiztm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/ggscfjhlq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gdpvumxtn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gdgzuolht.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggpnutcbh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gqzhotbuj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gjvxgpvnn.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gfjaasmps.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gfbynsbmb.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gemysincc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/guepihxtq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gkbmddfca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gdtekqcdu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gkzkurlqz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gwvwlbgze.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gpcogsvbo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gvyfpzkpc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gwmheagao.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gkwfzmopa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gniajgvpu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gmsyatwpo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gsgldlukv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gidzpzmob.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gyfvecbqs.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gnwyztaai.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gisfjqopp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gfjudbuhw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gbyxgfrfr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gyznkiqji.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/glygnkmdp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/guswwwezm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gixludetw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gjlwhzgcn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gkzxknffd.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gkcekpfni.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gwzabezcu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gyfhumzfs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gmximvmrt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gsdbctgtp.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gnihbccns.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/ghaggcxih.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gaigbkagv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwohrjvul.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gmwgviujs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcktnejth.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gtiakkyzc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gctdpulfc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gfspmdbud.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gwpbqjolg.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gxfvzlyqv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gmozyrool.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gpaefgyuq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/grdfeuxxw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gnjpxvhqo.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gabymzahx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gjgywygmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gedcwzmce.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gifrmwrqv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gjeotlefw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gnqadaavz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gcbhiyktd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gtwmgnsgk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gnnvxltau.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/grtebikpo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gcolxylal.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gqmhqzfzr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gxscymftr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gogbypnre.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gidnesbkf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gbcortthh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gvwffzzno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gvtdnrmpj.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gxvijaair.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkbxwscb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxchcsyg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gsoesmvxk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gexnbubwo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gwigbgwhk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gtjkvwhtw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gnwnjsfet.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/grgkxawhc.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gccwlabhx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/glbjulgsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gobfnlzyo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gljphyqdo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/ggwcrfzdt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gkruavomw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gauuhtwhd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gqhppckyi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gbnhxurvr.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gfisolarv.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gmjniarlf.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gczllmtpc.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gnjdxnmtw.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gwzglpvnj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghzocoejo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gszbkpkof.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gfdtlsspm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gvhkcelwr.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gwhkutajr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gjluhsuzy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gunkgejkc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gwqrlukec.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gmgntecpe.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gmhesejfz.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gsolgqlui.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gczzktien.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gskdwasbe.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gpuuglzoq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gtahnanmz.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gesrlskii.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpzsqhvbq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gmztneqtf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/grmkpcsex.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/glcsdxlza.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gslqrhtoa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gguhfphay.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjutapkhv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gvvbadxzu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbpclmgnb.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gsymjpzsc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gnwagyhjf.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gmllqnbnq.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gpwdkrcbd.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gsunkjsma.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/ghxyzfwgu.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gqgfsejua.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gkvxayuik.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gaeifdyxu.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gvbgqilap.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gjuegtjtc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gppfwxjda.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gmoydwymg.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvbxjmedq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gcfcjlkcs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjfqslmkx.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gnpirufwb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcvykcobc.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gkzgtatky.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gmaupszqk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/grgzkjxfg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/ggljkjgzc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ggtvtiyuu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gqejhvfry.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gsaorbfub.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gdkfhlvgg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gpwbwnndz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gvwcaujkq.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gtimzeypm.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/ghbazdcse.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gffagwced.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gtylfdfur.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gxlsykpum.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggsoteynf.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gfxqewlfx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gyctjdihh.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gcpdmokdr.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gqaoxecfx.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjjqisb.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmvmkahnp.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtaclzeem.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ggkwgscuo.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gwamppmfj.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gvdyibiqx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gomvjbjqh.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gwhjcrzxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gisqtwkey.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/giomykygn.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gwjrfdrmc.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gcruhjqqf.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/grpbsvcmx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gwmrpvtkm.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gbbfhnpoa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/ggexjlyva.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gzezuqaaq.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gbxkgwwsa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/golteyxsn.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gnhgpnkxi.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gegujzypf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gfwjaiepg.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gswbqauuk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gsqzigkek.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/ghflgmoqu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gkqjsnmgw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gauxqjuvr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/ggiswkcba.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gewcbjzrl.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gpywhvzrl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gihjnbipr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gnkbyxttw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gjoanyhrt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/ghagxfkiu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnkdepmeu.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/grswjzlld.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsjryjgqr.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gihipxhlo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gptkjbtuh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/ggonnxteb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gichlhull.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbtihdqvc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gemntqovf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/geshtckvf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gdchovjhw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdvrodbtu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/goezqgxni.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gwyktcwce.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gnlnncfwo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gjdgyhhze.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqluonmij.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/ghbidfjsa.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvhbirycg.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/giprmmrev.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gtdoedvvv.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gtzqvwwra.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gqyatkrqe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gifyzhflq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gezladitv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gmbhjdefi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gijgtquqc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gyiulhguh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gguuoaaov.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gttkwxzwi.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gyusxpzex.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjfcimuou.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gylqiolxm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gbmjwovty.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdlgqithe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gbjhudkdl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gtrgzntpr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gkanoziuu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gqylqjmto.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gwdtajqyk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gjwjwnkoe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gslnhlqwq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gmoalpgds.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/guiefvcct.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/ggxtcqwfw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gqxgrlzcf.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gfgjcdbkw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gjobfygtx.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gnrghoczk.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gdiduftwo.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gsrbtqtlu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbcuvzree.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gwoqajyrp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gibbjntma.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gsvlvudfa.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gkaeazgoj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/grpticdxa.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gurboyyxn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gjxwllfsl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gfkbwcfeq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gzlxlyzux.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gonitlgfd.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gsuykjfac.sHtML


<!-- 参考信息 -->