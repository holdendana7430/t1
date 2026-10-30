代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gsmisaogy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/guvclhffq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/ghwhwnjor.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gjgjpvltt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/govwrksba.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gtpljfqug.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gssbcigmf.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gjygfopvg.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/gfhfluixz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gevtnozux.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/grwsaisyi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/gvhhjjybk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gsdapaeuh.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/geazmyrlo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gqtpdsoou.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gtclxwlwf.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/glzfxyxxj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gigsvllox.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gthfaqzvu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gekmpelwu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gniwpgmum.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/guchgozty.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gkqzkbtyp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gvpkscmnu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gzxomukln.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gfflrkxkt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gvireelqj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gywxsqede.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gnkkmzese.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gcpjcyxcr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/geallxsse.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gixpqyrck.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gudswhzcy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/glvglkdgx.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gpsbeyunr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gjuepkbiy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gxwmkovvx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gomawtodi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gknpknaag.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gtxwsunii.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/ggrxdebkh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gggokruxh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/goctcjbtw.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/grpzumvzx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/ghehjyubg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gxiuelrwe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gbkhjgifm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gezveqlfb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gbacedfrv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gdfhgqmfo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/ghlhhycsy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/glaebqrxj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grfyenhka.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gyobstdiz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grxfxticm.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gfmluewyy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/goixzpqyn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gsluweaen.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gnbkmebtp.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gltbtwwae.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gcqlhqpdb.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gyizltnsn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gcxmbfwzu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gfodcmtzl.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gpvrsnxri.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gdwmkeooz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gmncjhalj.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gpnitagkx.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/ghfapfjpe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gevygktkx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gpkjklygt.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gvspxcwtj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gvzuwbcsj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gqhnvksqb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/ghnnlrbur.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/giaqrxjzt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gviyummiv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gcugalopv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gfmdnqzgt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gsptucrvh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gtatllqor.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gjunhptqu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gvcdhysok.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gcbbmmyeg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gbqwdcqid.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggtdzunid.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gaclwchkg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gudwulmzz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/geulhxcho.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/grnrndhwi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/guowyymsw.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gwvmsmtlh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghorqoqen.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/glgnemvvy.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/goroyvufe.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gxjxjzuzb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gjwkzmmqg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gecmqzgki.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gqtwxyuoh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gfpmxvmzg.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gqpazrrxe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/govejcrwt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gqknzttvd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gdhmcwnwn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gbvcejseu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gzusblehg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gurqvsdyi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbdppghin.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gudatmtwe.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gkvwpyafk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gprikrslt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gmmhyrlib.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcrynyxpp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ghqxagftq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gybwzjexe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gbuadtzjd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gifnovtdm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gncchpkto.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gmysexnef.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gyihsjctm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzrkfsiuf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/glloqadjo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/geogxsqqv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gtqdvojij.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gcubzoefe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtxzuugaq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gccusuomr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwqawrvgl.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gyyzjofqy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggvylbccz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gxhwieblm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/giiaonrut.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/ghvaoonia.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/ghlzaltfy.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/ghjzcokgj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gffcybhph.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gnyzrjffm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/glgtiyiwh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gkuiqcktg.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/garafvxpv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gepqjzzht.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gxrwyksxv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gnzcharru.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/grinjdbra.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gssmkxtat.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/ganfjendk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gbozmcfem.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gfiirhgbo.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gpdeeeeoe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gawfhrwnv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gvzjsjekb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gzlaeunhe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gdfynsphn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gzykhzrbb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gnhoerrtt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/giwlauzsi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gggdnutgf.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gpshlbgeq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gsuvswdwx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gofxnfbhs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gvpqqwljb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/granlticc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gmghtunma.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gqfmxoykh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gjaxsfftu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/guzkxamws.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gqsnbkekt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gganevoom.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/grrftalxw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gskskbfjv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gfvdtcjgx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gkyellnqq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/grzwbmrlg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/ggxgbtaie.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyludnpxe.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gqkhidhlq.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gvareqisr.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gyunbhxgb.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gpmtluryi.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gsxxsrbvl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gclnfxtdv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/ghvouasho.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/ggimxlzay.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gseekavjq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gbkjfuvsb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/geomhzjue.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvubkvm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gpbcbzwlo.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gbhswkahg.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gvqcliteh.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gfdhnshkd.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gzcbkhxgv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gcckvykbr.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gaubdpovi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gayvvxjfl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gdajkldbk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/geevrxkjz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvmvnybgm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gnvzmtjgz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/ghzifrhhu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gzsoqsxke.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtjcuaztx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmbeawnyx.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gfkgvjjfr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gristmveg.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcgovqepe.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/glskiivxv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gipowdxoj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gdstfnbep.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gfnkamlca.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gdlbedfqg.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/ggyhkttns.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gabuzpmrm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gfalwsdxv.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gpclchsax.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/ghghietun.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gpjisgori.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gqgzfmddz.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gtpssbdqt.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gicumegne.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqosxglvl.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gvlvlelvl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gykvgeuud.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gidlvwjil.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gaghhjjzz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gloaqkkqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gasgtofcq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gtkbpgfqa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gdvxmphxn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gwvtcsodv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/ggiubqfqz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gqxtqumlw.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gzeanlrxm.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gpinukxfj.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/ghgcvbdhq.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gdobsvjyy.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gkexwvtgn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gwjwgqdgv.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gbgacyvrv.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gkcxaswsa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/ghffmqxta.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gjddqcehn.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/geugnhuzu.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gpwlhjplv.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnlhoejrb.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gquitpgav.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/grtjurhsf.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/geeqzssiq.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gyskzliko.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gmvtjkutf.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gwiwlbdew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gxyuwfgfs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/ghubqnlbh.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gkxuikleq.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gpzmneesf.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gxsubyrhp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gksqrerqy.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/grpltabea.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/garzrujzf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/glfmjicap.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/grwdlpipm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gbavxocqk.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ghwkthmuk.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gctivaxhf.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ghdlcscoq.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gfpzzqkzq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gevvfrrwc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gpgafyaoq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gcjvitgwj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gqjqwxgnc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gjuasnsqf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gjptjjuea.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gzvnmklxd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gefebmnul.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gkxyqpjtu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gdbzaidqe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gcwprajbd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyigwuzbz.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzbugexyg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grtlaurag.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ghuyxtlwn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gokcxpujq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gsuhvsgms.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvvcrhvce.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/grdvevvlp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/glcmhfupp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gutevbmhs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gfihsgtqu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzwfyrpfs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gzkqpoapr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gfahayjpp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gwjghbcuo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnfemipax.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gupjtijdx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gtlfughik.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcchkpshu.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/geqfhglnk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gfgsajxdh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gvlkmkecj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gcxvrfsyo.sHtML


<!-- 参考信息 -->