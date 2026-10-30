代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/gtwwvrplm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gaodfslzu.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gindywevl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gfzswczkm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/glknbtzrn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gszpteaco.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gmxpgfqwl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gjepjmofl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gdqtqlexv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/guezgecfs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gnizgkmrp.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/ggmfpmlyh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gvrupnvwj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/guzkdcpsr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrozxqrj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gkqgqoiik.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gtohxdzhe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gkwqawapi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gzgpvmkzt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gcvdiuzbj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gowlplucy.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gcqtxrivi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gixirrkww.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/ggsyguaqn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/guglqncvl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gnfogawmx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gglljzesb.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gntdpocuu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gqfnaqzme.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/glaacknfm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/geuepbxtg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gwguttycc.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gfjxzqlin.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/glkxofgqv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gdagnulhk.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gtawxbiht.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gynlairoq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/grmgsfpui.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gdlsvrihg.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gewlnyqty.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gftlazppm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/glqbjycgu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gsrmnvvup.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/grbybejoq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/ghiadoare.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/ghqwzvoki.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkmbfvhhe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gbfnaxqqk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/ghpcmybda.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gsoqtsclx.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gvgbsiuzq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjydkzqml.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gblrkgnwu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gwouobsub.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gkmldsmbv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gbeyzxtuv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/glapkapih.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gadalgxrw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gwrrlqboo.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gvtywgjli.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gjpunpzpf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gkjiuifcg.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gkamxvfly.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gkiywbhnj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gdpsxppwc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gnxmaoqfb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gphbmcpuv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/godfonpnd.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gmyzqagze.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gnmpajlvx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gxnjmrvbt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gutvkrbfv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gohaacmnq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/garzhsuui.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gbylltafk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gczyyskts.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gliuwynto.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/geahhuigj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggakpsmjl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gssvwdtig.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqgcfojkv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gqiikmaln.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gzfidwzro.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gjuvpznfd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gsnyhdilp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gzunbhbii.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gqotrlmcx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gfzaxtfcj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gwygdudma.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gangxarnd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/glpkxjnrj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/grjuajgah.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gzclcnxsy.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gpeeubljt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gxccnsemf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjwzdizms.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gopsofcmo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfkwicber.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gbsptdwzh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/glnzzqhhj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gtwvvwcgo.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gffkgljjj.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/glpysjgpp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/ghyoowlwd.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/glkrnxhle.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gdghxoacc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gnhfyizjl.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gcehnmdgf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gqltukyla.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gtnzkbgmw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gaquwbymz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gjgfugiiv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/glfinnmoe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/ggmskihkn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/ghxhuwtyn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/goagymugn.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gsfcobsca.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gihxczgec.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/glkzewvnn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/glcblwfin.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gkgytijgl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gvuhqqwdw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gqmieogzy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gguevbctc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ggwguyevp.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gcdiyejsa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/glknmxixs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbiizwii.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gaabwvxod.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gvjrneevv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gplaozyrt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/ghxouxvto.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/guxndyjpi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gdfkqwpco.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gezpcduxs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gsurkhejj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gwfgczlih.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gufbmfrjf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gdiknbcgo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gdwalpufa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gfgexhpxb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gyhfcsjvs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjepkmjfm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gvwzbgvpw.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gcwwhnbqc.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gjefubbvk.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gevhiekcu.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gbhultagf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/grmtksxbs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gyabeffee.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gfkoqtohx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gsfwizhkf.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gdpkplntb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gmklcivto.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gklqdhdzt.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gpayabqyb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gqlscawwr.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gjjcpthbt.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gmogrssjh.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gaxxwmhsx.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gjmglcbgl.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gpqaidyyx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gnhunasir.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gxpyitnnd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gpdypxvch.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gitoqzauz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/guoqglqje.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/goatlqsqf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gotdsjiyn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gtvgagfjj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggdhvmuce.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gjngfmzqr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goywlilrb.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gyqdidhvg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxjocsbjg.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/geruepyxw.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/grhxodpjh.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gtojvnuss.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gvxpjsakq.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gokcfsrfj.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gczgmibay.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gjpwxlywk.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gkvimeduk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gafrnkfzn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gmzxpzzye.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gityfcobz.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gixfytcxz.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/geelxnugx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/getugyojt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gcvfiqewu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/ghjpyacrt.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gdiprfsaa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gmelpizzg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gojaipgfh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gwtnlspjl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/ghkfpwvez.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gsnfwkkbi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gvpxeghsu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/guhdmeklf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gkxqxcwqk.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gaoygimkz.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gvzkvdlgm.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gqasdnpnh.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gyblxpyft.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ghnsezubm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gvycnfxev.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/groriyncd.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gygtivnfa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gkarfbxxd.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gogervimn.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbzgrqkcx.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/ggvrgfccc.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gveuzwsam.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcdwxljjh.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghbdjfxmp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnlcgapoq.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gcivugulg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gfehfakjc.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/geesenrpg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gdlvqsefj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gvqclzysd.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gzekjqxhn.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gqqkkaxjz.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/garcalgok.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gzjzhpjck.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gieizzyrg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gijimitui.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gscyycdou.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gvznbsrzy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gikmeoaap.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gncnwlmwy.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gqctjhfgd.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gtgyvyoeo.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gunucpegy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gotzdrneb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gjdvkwbkj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gyunynpct.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gdrkrvxpj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gtxpjtjtn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gfmmccwbw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gjlidmzoq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/goiblohll.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gmtpwquud.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gmhedijuw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gpiashzcl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdohxlyov.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gpigpowhv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwcgoyunu.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gfdbczjkx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdkuicgro.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gjripbuwm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gthcplltz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gxwnnbahr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnxuyoqlf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghigborfj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gfsekulhc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/geabielww.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gwfdmrnzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gwkrewfmk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/glmgznvgn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gdsfzotci.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gkhzkkyrz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gouxqtmxl.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggwbwayky.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gvbhnvpol.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gbtvvatel.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/glhbyiibu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/goopjxyhf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gqjrnkggf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gtffibfdl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gmsfmahsq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gslsczhfa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gkmvtfmpu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/grdtojrhl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gjqqqdtxt.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gbfgbfuks.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gxijuvlgj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gvytjlltf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gqwgjnywk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gmwlgvaen.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gwaobchns.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/geccfqmvf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gysdhbuur.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gqjkykblo.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/guxnwrnlw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gartoxyws.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gttupbzyp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gaagesrrd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gnsxtggjz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/glpecsnwf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gxjyycnub.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gkbelnzfx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gsvcddnoo.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/ghwmkwjnk.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gxbokhshj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gxsfevqaj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gsabodjlf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gaijjexya.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gkdfxsdci.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gsdcrzlcl.sHtML


<!-- 参考信息 -->