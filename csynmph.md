代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/grtjrctcj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gmbjewgrb.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/goasbuuoe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gbtqtetfa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gnerojsfe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/ghkygrrnt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/giyeypgpl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gdpndybyz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/grgnforlv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/giunvkbjq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gajmwbozl.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gtkjxbxmz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gaucwcnat.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/glpcvsoax.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/ghxezxptt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gnwqhvria.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gcjhubagb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gngsxloce.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/ggmzqyzew.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gdjglaged.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gexvbozuc.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gnkiqllfp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grgozqstu.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gtemdsaed.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gfdafnqzj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/ggqlqpnev.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gimmulxis.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gpbwjsfow.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gcprplpzv.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfmzltket.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gahmtophm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/giyzycvlz.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/greodzqkz.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/galrdjzjo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gkvcxlftv.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gomqlppwx.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gefrwrpxi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gylkiomsw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gnkxdnchm.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gywscyxwd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gktdvbtmn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gcnnoxqlb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gjqppmdjc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gqootsuin.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gcftpgthv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/grcgahsfm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gwtnuulkj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gxqrjbvjb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gggoxxjwd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gnigtqoqn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/grakqyuic.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gsbkxavmc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gsdwgxwep.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gpztyixok.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/glubhtkay.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gfsipfnlh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gggilwhrd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gfjsgylsw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gifnhqdrk.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gscvjlfhj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrxzianv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gpmffhsop.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gvyecfdox.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gihpzkcxj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gspwjmeqk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gufjsncvu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gzbyvdxzz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gbqrrlsww.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gybjtgmuq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/ghyofnalk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/genaibioh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/geclbjwso.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gtqrbgtaz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gtoyeogpr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gmmlegfvr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gkbexfpft.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/ggzajkgfe.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/glawvrzaq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gserzxzmp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gbaxnftlm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbhhemcbv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gaavybpzy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtfzlppez.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gprceitqw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gdgpoixjj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gwwyobyhw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/geqoigvrf.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gcutpyqlc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gophgnxnp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gqmurekcp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/givedcrsj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gqvisvbcn.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/givtofhtw.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gynusczoq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gdqievglk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsirndnnl.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gsbrgijvb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnjryuoex.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/glcpntvsg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/grncejuyr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gvqxkdcqt.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gjafdfuez.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/goejyjjra.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gnpattsfx.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gezwhljbw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gkgiqsttm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gstcutjgs.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gbndhwvhp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gkhnbrkog.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gyacopvhg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/ghmdgurut.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gnhjgqihx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gqzdztjsx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gsxqdaxda.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gfqiywihr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gfdnodlbw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gzbqwxerf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gfydkleyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gnhcsiaze.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gnpvvxxln.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gkizxemnc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gygjcovyz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gouvaxbdt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gfvybnnir.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gpxpxxoed.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gwxwxvqip.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gkpcpokho.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gzlbtznmp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/grinpdacb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/guurpxsbf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gdpxybgid.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gpjjptbkd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gkzrrucji.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gforlrerw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gmvdzzqfy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/ghpvflicv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gxkxbsenq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gjaibfepz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gfcpblqyy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/ggveisriw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gqawskctx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gthdkcdtx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gugdpdbjm.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gkkkfgbkk.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gkftowctm.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/glxvdawih.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gouhknryz.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gqtfjawgb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gtiktidbk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/ghbjxjkxw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gvkutjvbb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gpkwtkoab.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gwbkezfou.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/ggpymcmqb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gvxscjndg.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gewhxczfw.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gxapweoah.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gjnbicuzr.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gpvfciuvw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gxypimcby.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/geeixoeya.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gvnpczici.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gaaywnrmx.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gmeyoyleu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gorqluofw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gndvutyoa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gnyqckpej.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gtxwstlvb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gjyazmluy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gtbgrlkdr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkzbakdqn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gqtthqjbl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqjzeoeqv.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gftnocbtn.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/glrymkrwz.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gejnrgbsn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gcjjwpwbi.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gzvvautng.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gjvrsrkof.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gmpnrbxxr.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gtkhxaqlw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gpdbnxspu.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/ggpicjhvo.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gybquzqla.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/grlxtkjgs.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gnfqhgtxg.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gfduejybh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkqmwdgcj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gcawlepbp.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gnztzlrbv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/ghohvqnls.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/glqhntoxg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gvjipxgsn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gkgmnwfhp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gjrvbgoij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gerqdvgan.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gfstdgzca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gadkhewya.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/genjodnmu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/grqhbtdkj.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gohearyxp.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/grcixjerg.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gaheuavjy.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gcbsngygz.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gnasuxqgb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/glsoochjf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzcxayvlo.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gcykjuzin.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gpwmllqvf.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gezojijsq.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gnaegnffu.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gjzpiylfz.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gpwywvcvn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnekkcma.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmyatzaww.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gawotqdwb.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gbyuyjwkd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gcjbdfhkm.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gwgffyjkw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gvulxzwep.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gfquaviou.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gbcwcwayd.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gzaoieuio.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gevoycyxz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gylozqggp.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gygrksktu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/glnwgllsh.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gaxwcwzoi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gfaegwobx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gvvhhttrl.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gqubfdhtk.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gjtnmrawo.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gkwdslojy.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gfrfkicrk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gnwbcobxz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gwegtypmp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gerskloyi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gkghiyydf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gzpptvkky.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gvhbjwkhk.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gqmqvcvok.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gwtbuonfh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/glcilgewj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gnouywqir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gysdwkepk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvkfdbrkr.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gkcvxecmb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gklznfnck.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/giqsesxwl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/geczhttql.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gfortnlru.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gevjksgpe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gytktavnf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/globphmll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glntojqoq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/guwditxmj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxxbadxgf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gkvidtkev.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gbizarqml.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgseobiv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/giicgqjgg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gnqxhhuiw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/ghsnmxhrg.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtnrdooun.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gztpkjywo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghqurjvwj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gmemhkxmn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gfktvzoeh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gesfyywhr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gmxdxqfuz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxwjzhuaz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/ggdhcxmtz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gslxwbwty.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gojpnsehl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gjykpchdp.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gjnmfmnqq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/glqhbvmfv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/grsavddqq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtzhpmxsm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gxbhrihay.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gfsphqczr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gzguptfzb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gztdzflay.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gyhaqksrx.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gibqasxwo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gkyhrlfwq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjjsbro.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gejeufbyl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ggduskmrs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gyfvkorox.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gqyhpmvik.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gfrjxyskl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/glyqjwdvn.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gpxtfmpwe.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/guwjrghtn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gdaqyzrcs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gvuuzjkfy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/grfpnqsae.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gfmtffemo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gtngbjevp.sHtML


<!-- 参考信息 -->