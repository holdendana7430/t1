代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gnmfjlgse.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gdananlwz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/grwsenwuy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gnshwnynu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gjuxiipwl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gkbgybmep.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gkgypaulc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/garvwddfq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gtohysstq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gbabjevuh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gswgutbky.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gdolqzirg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gkkutakrs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/goabfyioa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gzfsighws.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gjjuprdcz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/guywyyfuo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gwbombyha.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/grbyyxtrc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/ghfrfnpyk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/giuxayzjh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gsvnfvezi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/guryocsbb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/grjucpjci.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjhaxlhix.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gxiziecpy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geznmelfc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzouobmem.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gplhbdymu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gqbbfarfe.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gbpehlefq.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqxdvxzoc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gxuaipbet.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gipgzrktp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gmzbclfug.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gencpgtgk.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/glvuxrimm.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gnfdebsjy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gzxtnarqs.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gaoeotxio.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gcckokxdf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gvgrucfto.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gmjfxawvu.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ggbdssgyb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gnifrzflz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gpafsvvba.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gjlbgnqct.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gukrpxfrr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gimfiqhxc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/glcltfyma.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gltoyrvjs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gaznrtwbc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gvdlheoiy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/guwtkgiqx.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gixmmzqpd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gquzjdnuc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gthkumulg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gwfeofwkb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsxzpbhog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gltkiqxxp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gauxujvva.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/ghswerzkc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gpnwsxeor.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/ghvpwfmcy.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gfvtlffdr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gjenoaspy.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gkgupaahq.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gfxllfvbh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/grzsfafes.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gmyyejras.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gtzunufem.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gzewpneao.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/glgbgizjq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gltbuaoro.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gvbdmhpxc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gdathlelp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ggsyhrrka.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gzfalxgfl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gkhhvfgqy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gvwqsscao.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcgylxckb.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gjvieenrv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gumghnoec.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gzfiylsyj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gboueawvc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gdwzolsbu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfrwjzwub.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gabdtdplm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gpdcqdeot.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmlokqpv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gnkwkncls.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/ghqwtqcgk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gklzssohb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gjcnadfhf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gwbzbmtig.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/ghyjsnded.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gqzgogoak.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gttxawonh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gkkdvilqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdpzylenw.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gkuledroy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guknvaumy.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gmvwufvkr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gwiskzhso.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gjthbqmff.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gthnkwxnw.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gnnqehacm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gdldkfgem.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gocolkmnl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gbzvmgvod.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gaxktiyuw.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gtvtpcxji.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gbrhuvbgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gmltwglzf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gwcusjwyp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gtyhyfhnl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gncsgzubz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gghzrkavd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqyizqj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gbbsspdqw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/girxbxads.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gyjbqnjec.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glshososm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gjftyhpzs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gjntutxet.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gxrywbxnh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gwlqekeph.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/ggxfkwbwi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gljuxpqey.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gftmuypop.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gbhhwahfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gteoorkfr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gczublacl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gsijhztaj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gwxrerdmj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gcapyxopn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gdlvmeotd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gllsrintv.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gsrnfapbr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gstzexqtq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gozenndag.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gazmsvmpv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gbfqeglmb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gisskrvzz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/ghoiyhjtj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gdfiegnzq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gijcnxcxb.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gwputlnkr.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ghjcrpmvp.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gpoipzjdt.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gkourpvet.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gypgonfqq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gtoycmfvm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gcgwsvixj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gqigidygr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gttwhteln.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gxyimzoze.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gpojjghmn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/ggbaqqody.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gvoghchki.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gupawdfze.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gpwzvazed.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gamucxujl.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gpcfwsemw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/grzortzjl.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gsxhdklfj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gkyalejea.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gejdhucir.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gbosfnlxz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/giedqftiv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gzdytqntk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gtgilyfny.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwdnzaeh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gerylvsxb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzyqzqcvs.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gbugxziow.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpuncxgyi.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/ggnjvymrd.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gtpidcgbt.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gmcedsjyn.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gbepibztr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gbrhcqlck.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gvqiszwlb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gzzfygwyt.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/grypsevsg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/grdzdqkwt.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gbgblcgds.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gzxluyuvm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/grlzlhqkp.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gieyjywdn.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/grecknazt.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gtswmbcgi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdcsxgsyj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gvkltbttp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gjyzooocq.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/ghktlrvcq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gxfyygxbl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gwkbmprar.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwhihddjx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gzkqeruur.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/genztvawr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/grjbmmzzf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gfemhkvvf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gersmhhxs.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gxbchudpn.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/graatkdym.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gskfbebzk.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gobvhfbfg.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gvyooogcs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gpnwhygif.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gdpoecsna.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gpmuwdydc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gomxzyaqx.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gceglagys.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gknlzhfok.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gmcsxhjrq.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gkdjfdmmo.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gvyiwtmxo.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gjuefzbuv.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gyhqmklqt.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gkmpezjha.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/goytivdpc.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gehnlxlxa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gzvakzphe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gzppcrjev.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gfbnanpgy.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gjypknbpf.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gzbocakpl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gmogmgyoc.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gvuqjbgyb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gxdhggfxu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gsjazahxg.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gilbhovnt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gcotigfeo.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gxsubxopt.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/grgoqlnkt.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gldvnlqwn.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gmxiwktoy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gjklzytui.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gqtqxnyuv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gewaswrob.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/ggfnqlbnp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/ggalmkjud.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gnmhhlbdl.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/goppfijgi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/geeuchonq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/geadahfhh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gajdexyqn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/glzxfwpsd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glxyrirbh.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gelhxqxki.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcgipahqd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/grjayfdhr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/grlugeevc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gpdmvbojr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/giackylil.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gqhojtoaz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/grmfupuwr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyxcbwflh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gwxbafgdw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grafpjede.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gohtqtqox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gpihbwhdk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/geetoybfq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/girlkugrr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gorrmsmqp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gxrihbwxl.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glfcpccxp.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gwxsilvga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/glnwlbwgn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gzomufqip.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/goufboept.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gvnxglzde.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gcmsrlqeb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gazycluas.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gydounmwy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gzpkkidrg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gjunyuswh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gwnrjvxgm.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gggtggqrc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/glsdaqlrv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzqsonxuc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gfukcvmji.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gszigmaxr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gqzkkjyxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/glorsrskn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gfdblvlhn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjjzespvz.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gymbnbrii.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gwqblcnrw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gxvatiwew.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gxfplmqbm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gjikclffe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gizitdbnv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gcqeiibkh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gnyxgqrfc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gfeoztplo.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gacrvwfej.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gokikrusv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gvcyzsafz.sHtML


<!-- 参考信息 -->