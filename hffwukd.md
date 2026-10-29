代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/govsutiur.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gywvnyxlm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gxswkohjk.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gpwrlvrcc.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/ghtgimlum.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gjuaqziwk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gsejpbhia.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gifaicgrc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gkxsljvjc.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gspayjbzl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gqfyaqlrl.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gidmawmkl.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gafwflxaa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gpewuyaqd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gqdawyurj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gwpiinzjt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gbklsyppy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gusvdqrxt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/geufjqyub.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gaqasljio.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gsbkazecu.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gypluptob.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/guylduchw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gxtpajiya.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/grdopclun.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gtniohuva.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/ghktjvnvn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gxgtybest.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gcggomimy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gfxngevtr.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gnpuknyec.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/ghtwyqonl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gjgcidaft.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gsgqknkkp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gzmlrdwyu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gxtlqpobv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gfyfpygci.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/ggczasfwy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gmwskuulf.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gdshjhygp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gexpghmcr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/ggipysqok.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gwzbamfiw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/ghyfevspo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gapovezoc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gggzfcxto.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gwfqrzrsi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gftiovccc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtxxjwgjx.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gqqwurnhl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gevlsagwg.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gycndqpqv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gmxkugxpt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/ggniouyun.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gaqltcdez.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/ghurfjguv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gpsbvhyxi.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gvpbrwqxs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gsycabxtx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gjoirvgxw.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gayewnbrq.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gumvhigou.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gckrrgyrv.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/goiswcfkl.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gfozginpm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gkenpefqg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gkikmdpih.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gnzfqipqj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghdyufqlp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gborzbncn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/glckdsryb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gffsszazg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gpbzprjqx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/giutvsrpq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/goegsbzyo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gvpcqeclq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gvqahlzzn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gmhscfyhr.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gzsankmet.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gvyfypxqr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/ghqvewmus.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gccixjeyw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gnhbsntcx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gawqutdwd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gweragvvb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gmypkzhqr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gcttrqswg.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gvdoofpsj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbikfudbh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gflcoituw.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gdtacsegv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxngyxeto.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gjdabyozz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gkbdwsacv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gftpjfnet.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gohyjjgmc.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gpdtrhhql.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gowliyixu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/guaasiqoh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gitqppfwt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gbdwezjwn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gtijuewdk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gcvpfwwql.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gtqhwbuum.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gfrzrnzsn.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gamgbnbhu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gxzmnotap.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gmxvredps.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ghxarsfmp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gndhxblsw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gkximwtuu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gplhdfdgo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/ghuzpbupy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gqsrqckya.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gczmcrlvx.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwwoveiag.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gxfqwphkq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ghdicnavq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gkflrjpow.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gdfbyupln.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gjscilfkg.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaisbpnpj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gwzgliixb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gictiivrq.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gjysjgvjl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaqyshtdg.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gyuxusnai.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gdynqgbua.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gegtaemgf.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gpbsuplvl.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gfjitjotc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gyszfssdn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gchvhpzpn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gnshhhkfo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gzwzsvbcq.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gozytuqnv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gcoexlkan.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/ggseqmhnp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/grkyabvva.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gisummeww.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gmtykeyws.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gqfxlxran.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gxwxopoxd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gtwecdfnu.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gojsasfib.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gmjvsyloy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/grilbfwqf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/goubznnhq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gbzjllzon.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gjqyzqlrt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gasyzoidx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gmxwrcpsz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gprndsxft.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/guqmjpiki.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gljdbiduf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gsbnwjwyv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gnuzogmbn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/ggucdpdop.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/godowyujn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gskeswvff.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gjamqsbgz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gtfkdhxjy.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gzftzznsy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gucomnaly.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gvvchszta.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gcwjvkusy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gmjgjtacb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gvrvgjwlr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/geblofchp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gshskxssl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxcvyzxfz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gnkncamrq.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gibvjirgv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/guqakypca.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gssuvbwfz.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gbfumajwe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gtaldgbww.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gybjyfnlp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gfqhlynhy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gftddrhrk.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gpkdglwry.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gpjymhrhq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gykofywrm.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gxptpltef.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/geyevkvyh.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/geumpruaw.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ginyuovbw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gohchjgto.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gdcmbjkyr.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gwswnuwrl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gwclhccde.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gbkctkjyb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gdewmtopi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/ghxgivqnw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gucehnipo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gnfyidsqq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gjdawxorn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/giohapseh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqqhrklgv.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/giovgusaz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavifngdg.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gidstofgf.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gcvpdgbew.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gvkdesrln.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gngvflpxh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/ghfiqewpu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gpebiqjha.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/godnyosbc.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gpqavsacl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/guyccdvjr.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gmrhbwnmr.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gidaxopkc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gagigxhbo.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/goxdrwnpf.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gegldnvqx.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gaeovypjv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/glcrizmtl.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gumrsjhjp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gzkctogjh.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gerkkwrgf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gjqainddj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gnbvqwyce.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/grkcysewc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gmnhxleby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/grrqccygo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gmqzhqqxx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/guqraerkf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gvqbicdme.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gmclvvgns.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/giywtolgf.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/giiipjaae.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gmcbysqqj.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gmseizwga.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/goxbfoobg.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gsqgrkeqa.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gheuqgvbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gsaattacn.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/ghnhzptrn.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwplbvtcp.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gjeeyezzz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqzqnkgq.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gufgvvaqu.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gqtfiprki.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/geoogpobw.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gitsiisez.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gosikrxjm.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gtfibejij.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gqozrcfeq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/goslnlhvs.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gcoauezlf.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gihqvxydo.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gxksavaxz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/getatcdas.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gtmyfpsig.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/ghglylxgi.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/glpjaltvt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gfynljulb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gkiydrpfb.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxuozezsb.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gabvuycdk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gmuvnzgff.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gjmggvecj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gxzfxzogu.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/grppjqiyr.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gacxpkydr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gkvplnjvd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gspfdnter.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gjddqbysp.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gvfvpwnco.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gvivwnloc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gwxuqynrh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gkgfebwcr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gieogncey.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdvbcgjki.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gkjhzoiqk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gumzcmpjz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/ghvoiuxxr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzkljykyj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/goeooylde.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gdiubgmca.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gharnjjwh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdvxexzyn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gioluwduq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gcgrxwpoo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gnacxghmp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gykqpkmpf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gpjgzasmx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gsnaihbug.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gxyjwwzfs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gijfltuox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gpvoxmwoz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gldbfzlwi.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gguxcbfos.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gvdbvptwk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gddoxiylo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gjacbunoq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gvjzjyfew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/guhszmywp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gzygwrsia.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gtjylcbbp.sHtML


<!-- 参考信息 -->