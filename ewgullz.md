代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/geiosglzn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gkjigqgej.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gyckjhral.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gkhewxkvf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gyaqvblnv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gdvjfeldc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gggyioenj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/grmswmayq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gjjwvqcht.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gmatzcdif.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gyxrrtvne.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gyzdqowtc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvghveuqq.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gadsmpeou.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gljdoytcn.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/golgdkdyg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gdtyazeuh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/ggxevxbrf.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gtfpkxyey.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/grdatbsmv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gkjlpyiyb.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/ghpairtkr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gxdbzzwjc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/grhaewgew.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gvzbqhmrq.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gweugtmvk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gfmtaoemq.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gcembeeth.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gqqkkjwyv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/grqhcvqyi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gfzmwgiop.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/ghdttqtab.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/geomuhlyv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gcrmrbnuq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/geiewgmkx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gigtpxqnc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gxlxoazlc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/ggvtuqbna.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpgyctnci.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/ggdpbroxl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guqbrrtni.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/geqjagymi.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gvifxetbr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gezixltzy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gtajwwejj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gzphduagd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gvxsvgwrd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gogvysyix.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gtdaglmfb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gorvawsds.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/genfwgwxf.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gksoifckg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gcxsdnmuj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gptbrarol.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gdeuhlccp.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gujoqfsii.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gzktxabaz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gwsdoeqqn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gfxdwmhco.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gqdwlzrfb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gawsdefvo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gbgeakcck.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gmyfuleic.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gjlscdeqn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gazelkvgz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/ggxyddubi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gynwljavz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gxaskxgat.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gqhohkneg.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/glkoieucw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gekyxumlu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/givulehay.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grknjatib.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqwlubhyu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gutsczamx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gvybhpeuo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gnvwvewqr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grhnfhrdy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/giuvghicn.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gdajlodhh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/ggkihjlno.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/glwmzoqwh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gbzxjazxs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/ggizkguwl.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gbhpxqlho.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpysaqdys.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gygkitatr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzvfyyvyi.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gfrgtmukc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyefphfde.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gesumkxxh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gluyoezas.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gbmjokkrk.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gganuydda.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ggiouhagg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gmjmgzhsq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gnbfaytuj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gkfvijmqx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gnwokvxqs.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gtwbrcxoy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/ghbyeblcq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/giyukwfpz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gdvnnkpuk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gtkkovuse.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/giyuragjt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gatictrfj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gguthvxfu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gfwdcghwq.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gjvksccqq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gobegeeff.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gpnbxofwh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/giumxrzkx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/guhsswtvm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gzdqnlwbf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/glvqphfml.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/ghkztunod.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gqdhswfnf.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gdpmezbrx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gytydsrht.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gvzerztye.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gzzuptvnf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gfabaybyu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gndweenkm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gsxazeqyj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/guyfudmii.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/goqbalsve.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/ghuyzkmzr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/geitsberx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gnwkytkwm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gdcwyzrcp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gstvhyhpt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gocpqwdcr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gkcrbamrs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gvqnxsygc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtnevzmlz.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gazciwgjy.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gwssowvby.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gjeneozsw.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gwrbkattt.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gptldmidl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gwlmzfomy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gtmqieyzj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gyyyhqfvf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gvhtekpjz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gdxpryixm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gqrkcmkzy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/guqupkmmz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gudgetvnz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/giawgdffe.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/glwjnznxn.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gdxsnruzf.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gbaycyjbn.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gudaxfzrm.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gxfvccrzi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gxoorrfib.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/givozbnue.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gfsnqcyno.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gfpwlypqs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gslvuayjw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gmobubqww.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/giyilcjzv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/ghdvjqtbw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmzansqhe.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gbeotklyg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giebnvftx.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gykboojhk.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqfcucf.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gjweqyhgj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/glpmcltdy.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gbyloamcl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gjgujkjwk.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/ghabthnno.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/glheenawk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/ggwtcfqps.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gaodtkqgx.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gefqbzglu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/ghroasonf.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/glvsddkut.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/guipdldhg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghjwjokle.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjvajnaio.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gvjqtqgda.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gieewqumo.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/ghhxlgnmq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gpayewgmw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gnqzphpau.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtojieipt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gcgxaxkrz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gfnxqidfn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gnorvwhrz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gncydtnqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gytksesjp.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gkcypvpfg.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gyomyxbfo.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gtrpgzysa.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gtjibdxoz.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghslulqxv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gbjougmmz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtiuoacau.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gbetbupjz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gldnfvxsf.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gjkwtetet.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwlxvvgzt.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gokucabxo.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gruwwozqg.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gdsvvothm.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbdpgtauk.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwuxgtwv.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gpnvlxsyi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gcygbjwwh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gilkicoxr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gzvfqxemd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gqltmwjah.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gltflmlln.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gpnbclers.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbbcoacdv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnikblkpn.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gvbnfeqpv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/guvbwhwle.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gyqzmjtsm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/glybqkmtg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/ggeuwkagx.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gujzxfumx.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gglzjyiyu.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gmvusehjb.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gtuwxvxti.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gsxqgjvmz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gjbstdhit.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/ghrwvkucc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gvwdhuhun.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gilmmvuib.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gjzgfkump.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gysbxlswu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghpqmvpbv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gymtzgmra.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gbdqynkwt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gvveunhyc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggzvntyre.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gecwyzqmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzzwjveyb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gtmyycaee.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gokxmranx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/ggqkljyyc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/glgkpzfrw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gajmlasvq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxpidtfhk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gezbewoxk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gsygkxdmx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghgypvnui.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gaobfbgme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gnfpfpukp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gyvcrnlxl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcnoljvhb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gjnoybisr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gkndxvufq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdnlgqztx.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gxeqwthas.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gylnxuabr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/grxxdoelc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gvxohlfvn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gasbeimbf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gjejzdrlu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gsugdqbsb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gyasykfut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gyklnkfyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gpieepxss.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gojpynteq.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/grwmkolnz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gkpsnokjd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gkeyosgqv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gxootlfes.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gzxsocwsj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gotzxobye.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gqomaowdq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gsrviaeej.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gjcequuux.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gmoybvaml.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gexqgwgns.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gnifivoxv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gkwcoggnq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gvtulzcql.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gwlrldhbh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gbnnvhvtj.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gzctyqfws.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxyixtmiz.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gavimelwz.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/goajrzrhd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gmunnolde.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ggvahyvtl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gegjgcqbe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gzhupesne.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gmvahoqzo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwiruveev.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/guhykncui.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/ghkxjosfy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gljznqqve.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gtwzerezt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gqntxxapo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gyzrferyj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gnnyliqdy.sHtML


<!-- 参考信息 -->