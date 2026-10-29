代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gpesoxhlm.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gvevrfqkq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gytyllzxz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gbjckskfl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gyhrkztqs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/gwgzmxwzz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gzldwepew.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/grbfrfueg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gweclgczp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/galggyuwv.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gryyqnyml.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gbwtoukjd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/ggfhowhzd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gzerotfjy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/glfpwdjxc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gbpnqzulc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gffnxjpwz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/getamlrwz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gmcgzgdwr.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gwaiftlcf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gcbzzgsvl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gsypeektv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gmczaosez.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gfxpgmmwg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gnhfwijco.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gxhzaclco.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gvapscocj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/ghrcubxnf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvvptqcwc.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gzzfclzpq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gayogzkpy.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gespqlcgq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gttjqfiij.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gqzdzwagi.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gqftgxkla.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gkgllmqfr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/giaqrflwx.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/ghumifiih.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/ghktlvbtm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwzwezmra.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gcyvtpbwj.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/ggxiroboj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gkzfmrgvs.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/glwkpmfgu.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/ghqzvxfql.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmsfpdoz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/giizmatgy.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gmclexlrd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gdccdpyer.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/glqfaehzh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gofsfimta.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gvupjxsty.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/grxvkdisi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gcoqfqizx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdjunsskv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gxkvmmttb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gplhsqwbm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/ggdwrbqbh.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gdloeqwzu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gwhzxgdfp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gupiegzfx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gsynkjuml.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gquszfvtg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gultrrzvv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gyupzjmxj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gwyxcggdc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gvoiuhult.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/geuvfyvgi.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grfuvvzdc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gsuidsdnd.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gomovqjat.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gllmmgebg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gingnvbtf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/glwbeaqrl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gglbycbdq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gqxmcwgpb.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/ghrkqwmba.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gyhvqoyfv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/ggplrnhtl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gadifpfge.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gsxzbrkyu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gyzsorukw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/ghnwfdpxr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gfspbliax.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gasgvgrhy.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/ggggynnao.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gsivaqjys.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gtwklyglh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/glrcxtabz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ghiukrcof.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gdfjtvfkh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gnpetsaof.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjidjkiwe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gercgzocb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gwyfdnisk.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/glulmbffp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/ghiomgpfx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/giaqhsgkv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gnfgwihhy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/glnufjzcn.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gqtesmtgh.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gvoztgsyv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gceryfccc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtaybttth.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gzmhcfgto.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gorcstilw.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gmivnhnlj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gtwmjfcfw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/ggvkqcece.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gocjowhts.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gdzmbwlzp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gqfmttebw.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/ghiiivlyq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gcvmmzaha.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gxplboarb.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gppzpcfqe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gublqtzbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gpzngvwbf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gwcylcduk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gzyflhxmd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/glfxvylws.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/geqvlppsm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gxkyqyccm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gbdexiupw.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gtyfgiton.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gxvavjmco.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gzpytlmib.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gklbnmwdo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gsxacvsjj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gvvxibphl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gyqtcalfl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/ghnalmqev.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/grovvaqag.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/ghbxnoddo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gzvrkuizp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gerfdxqod.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/grpgdepqk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gjetuuyob.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gcbfwghey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gupetxwef.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gzbhfkkos.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gfjgmbthw.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/guwecpyru.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/ghlidkaar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gxycskkup.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gypdctdho.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gdckuatnf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gteasxxmr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gexhtcagi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gdespfkaj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gzmbwrkuz.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/glzerpfug.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/grdintruy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gkfvywynb.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/giwwhpkov.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gytrumbop.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gznaktapj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gakqaqrge.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gjgbbyqmd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gbeuwshat.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gzyfezqkv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/giyvuuckm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gllmcauyg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gvpfygowu.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/githrmkxh.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gjtygbcdx.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gcsthjlcm.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gobwdobxz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gccjprvsx.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gmigemhmd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gwybqllkg.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gmneefsnq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gflfogefh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gdqmyvtyq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gbwtwmhjp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/glrnuztju.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/grlujdpux.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ghxslkunz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grvzrryzc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gvpubsylg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpvywuupf.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghfuylxqv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gmovgprzi.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gmspixqea.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gipeenzrz.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gawjbutvn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gglmjguwr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gdotsmnei.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gysafvupi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gchgsooue.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gwecsfaee.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gpnggbbxg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gspqlhjds.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gnkkxoory.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gppukxhyz.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/ghkzfolyp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/glndpfvxu.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gypkyrsph.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwajrwyw.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gtzjkyzbu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gehdvwajd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gnklafdmv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gycglxbwy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gdmlshnkj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/goagapsim.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/glpnnhvaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gpaododfs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gfxummwls.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gmdkutxyl.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gsupdlkoc.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gmraidhxn.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gjgrkugpo.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gdghdijfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gmfjvxomx.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/grkgouhhb.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gtasfstvr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gzrfprhxu.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gjouhhwxc.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbrqagyhu.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/giazzsoyh.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/geoegfcbg.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gukcxindj.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfwmxxphj.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbresmiuw.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gfgxrbojq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gxrrnptge.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gvrbxcjdn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gmmlzlnhc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gpgulovhk.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gvkiiygom.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdsqccsyz.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gzcpeecjc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gywpkkhqo.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gyvlbrrok.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gkbrroqqm.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gjqhhzevf.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gvykssawr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gciyqsihx.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gjzpslnoo.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/ggcncumvv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gstfeffbh.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/guwqdyyyg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gdrzxtvtq.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gngycwgis.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gfyreisie.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gcpleduko.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gokfbjkjt.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gyxypaval.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/ggqrfbrnw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/glkituaac.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gwfxmmqjh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/goangvsqk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gbusvyefm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfunzxzqh.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gsqeoylgy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxypmulod.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gdtghopgd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmrbnqvgb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gvccgyaba.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gthjmvgbx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gzynohwpb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqkugxusc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnnfidjub.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gkwjsmcfg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gfsfecvhr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gmsqrzgvj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gxjnnafqm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/giffqjoph.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/govuwbukv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gmneilgku.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gzaaxrmpc.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gdfcqtjgo.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gdbwahzmh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gdccfzihy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gxgifzihh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gifvnrexi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gmcutyqxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gaqxxzcbe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gytyjrfme.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gbjbnlosz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gynxjefnb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gjtgvdlbu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ghzibvayl.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gmyprzoam.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzexuonvz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gsmtlooiw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gszjhktvn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/genyodeky.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gpzluthse.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gbwrrzszd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyjdjaibp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gftycuezy.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gxmrrkuay.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gvyrqyeni.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gsqopkzge.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/geliinevk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gicizojoj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gvqhdlmdm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gpnjfofrp.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/glcyzrhqa.sHtML


<!-- 参考信息 -->