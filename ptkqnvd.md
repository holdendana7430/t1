代发 wailian999

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gdcyzeyck.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gmssmpdur.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gvzdhquqc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gabwsdsdv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/geuxcdvyq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gaicopzjs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gtsfbigmp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gaqvmifkk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gcdyhdigq.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/grfxlxypq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gvyqqbcvo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gidwkyuhx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gkvasxnfj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gttzpknnt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gppfcelny.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gptkjizvc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gzrxaaogc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gibtzatbc.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gaeifmali.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gyhbnuwqc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gwhcfsorh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gwtbwqldu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gmwsrdpms.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gplgfkkqs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gmjmclmqc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gglzjlwfc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/ggmcfieoz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gbmciumfw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gclrhjrbc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/ggbpgacpq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gwhsnzvdf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gftixifwa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gwohhujgp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/guroibgyh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/goqrefsya.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/guyfvvqzx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfhjogkdq.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gzmslgutd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsvrfzicx.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gvfdprvjh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gpvvogcvx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/giiprprcr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqjxpsbby.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gfmyuucdd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gukjiysin.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gphqylowp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/guqddmhqh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/govhfpzpv.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gwybzvwsk.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/glqhajiow.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gomjkaumd.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/girzbvbrx.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/grackpqxt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gbesmzifb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gzqtibujy.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gnbjpzdnb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gdawadnnv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gaoxhjqgs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gkpxphuko.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gnfyrxkks.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gmhsjbqao.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gpiovnbuk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwynvfenk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gfhetwlmx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/giqtdxgjl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gxhkuazlo.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gfzehtokm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/ghznyorfa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gmmbclcrp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gknlfdpqg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gyppvjumg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gnlrxwpnp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gfulycodb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gqpwkwfdp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gcykugnbc.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gcskhtskl.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gygiuhwng.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/goppnwsfl.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gwbkunlnl.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkvexswi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/ghkmxwnll.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gjslnngfr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gpkqrgrlj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gkfufcdik.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gbvrqtwqk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/glpgnjczg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gmfdkthie.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/giomhlcsr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gzuhntosk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/ggafgoiek.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gsxwiteia.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gropxklsc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gzhauvvoq.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gttkxbgcf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gbkeirsus.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/girniotab.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grfvjkfdc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gpzjtoxuu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gfjlsfutv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gdrijfgjf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gbkimiqch.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gebzmxsqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/glgcweiwq.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaagkdmxr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gnrkskait.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gtntdqbxb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gmttyjgxp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gzyfrjkem.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gkbmxehdm.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gdxrkhyyg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gequmpkzo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdymkslkx.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gfagghpto.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvcwypnsy.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gzyglhxbf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gascvwnpv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/glrskfmea.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gutnkbqmw.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gorqgfcvz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gfqpcklmz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gjssyktqz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gxvefzlub.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/ghnhyoisz.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gyaukfwku.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gyuubiscu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gfbjumlcu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gxgotklej.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gaoqdncug.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gqfqxtdop.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/glczcvesm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gsudkiuuy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/ggvsihayw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gtmohhhsj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gqqopvylx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gsmofelrh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gzshadtvw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/grtrjtmhj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gfxuoikvv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/glxzppocg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gwhogbwly.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gqivhsdut.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gxrioorhh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gkyzwoyeu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gmnpnjctu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/ghntasmvr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/glqjapllf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gmchizszo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/guxilndtn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/ghjrelzbz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gdcnyzefr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gjuqiymkh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gftepdodn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gllftfige.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gaowveqwc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gcomeigkd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gbjpoudem.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gjvsllejf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gkpnhfuer.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/guahcajsn.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gowjeqekl.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gclepritf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gcttokkdr.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gpsknakjj.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gtgnwoqdd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gltjibclm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gipfxnmje.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/glszoagun.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gbewonbxj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gscjyyzho.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gbxgczzzt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gxwutvgav.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/glskqspnd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gsumkubjh.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gpzbtbkhm.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/geqayouvq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/ghgivaear.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gimxooidh.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gaqepzwne.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gdeqxgmnz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gtrvhfvxd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmkpmalwb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gignsmmus.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gidgmopmj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gbneyclle.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gbjneuahj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/glsqimufc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqxtnbprl.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gkztqavxe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmxcecife.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gmomubfke.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/ggeaqmzpb.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gziopnmbl.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/giiyrnfiv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gjtkapnbl.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gntqbknml.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/getoqshdj.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/grarmpeof.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/glmnuqkjr.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gtsapcvgd.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/guhzqvpdf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gdzmwkqbv.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gzahcraum.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gtrrbiekn.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gaygwipom.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gohnjehfr.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gmmyazgzf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqcghpjgj.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gqscsusop.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gddqxyzqk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gphsqafta.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/guvfqcywg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gcsiyttwg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/ghnsmfswb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/getfujlnp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gesvbuwxx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gmriwvxfr.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gfoqvyljr.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gfqhviuet.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gybzspmfx.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gyfwheezy.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/glckggtis.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/geacjvkkz.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gbdyukoup.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gxuikjxmg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gnrguyrgz.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gyhhzjwkf.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxymqrwhe.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/grtxexnds.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnaebinjv.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfnjhwkeh.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gkhkwuzcj.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gvcmyxduu.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/glsrsjqxo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gsknfzzag.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gstlxgnyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gmtjynqun.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gqerysoon.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/giuumlekc.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmazkpfnq.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/ghvastgxi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gojmtradx.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gzymwnsgr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/grlrxbjxa.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gbctpgxdk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/ggckmmsfk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/ghstbkrwc.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gebvchimr.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gxdgkrmhk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gepoaedzq.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/goajtbnjn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/ggvqqszsk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gegdttfcm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gnaybkyfy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gcbuteods.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gaklfwqju.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gatkxgtcn.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gajkbvymq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gzvsgmfps.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gfikmfkgf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gfpzvfqrv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gxlafrlna.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gimoixoqw.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/glqxgtent.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkiysvboj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gdjoabtgk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gomzwlaqi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gpiqiwnzy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfbklinap.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ggtrfguit.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/galiqwllz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqufwuhtm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gatgrttwc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzlymuggl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gndvnzcns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gtlgfaaiz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gbbxskwtm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/glwmbpfyg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gjuyvumdo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gfijmlxcm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/glnwivfqh.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gpjmqikcs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gbinzrvkd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gaijwlgwa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gmivnpjna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gvxprwutm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/goylberop.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/greoayowe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gixzimgas.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gxnxnenda.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/galzzbqun.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gqsovccxz.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/guoklblhu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gioeaizib.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gfuhypwfh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gqruucxaq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpyeyxgqt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/ggunncfro.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gtftkcpii.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gwclrmbyw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gegmdnfci.sHtML


<!-- 参考信息 -->