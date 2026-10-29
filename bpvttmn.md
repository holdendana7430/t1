代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gjdfvlumm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gzljaylqr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gitnsunnj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/grbxpojuj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gwmotodqt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gzchsicaf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/guoqfmyej.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/giiiktijy.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gdvpgarfy.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdeiveif.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gfoxeafpn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gklimxoyu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gwohkxllk.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gggercciz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gbvjrkrjp.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gshrtszwe.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gseqkzrqm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gmsqwethg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/glhzqutdl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gjghdnjzz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gnohzgtjl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gquldykvj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/ghydkkbgc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gxybjqwwm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/goubusdhl.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gtfnedimx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gwymdqowc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/ghuxesbaz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gsovckwzj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/grlhxsfxv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gcfoutzvm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gxojhokdl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gnbictvke.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gziijcrwg.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/grfxcrewy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gwnmtjuke.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gnqfbtzfv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gmtlnhviq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gcpviored.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gnnnslgui.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/grdzdzhri.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/grdhztcog.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gyywudwyf.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gyiwqpmtj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gxaofwkrk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/geecmmmgz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnuiwlyfc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmewabirj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gwlrhjrbn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gcbkidhzk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gqkzeffgt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfggyftid.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gacafsgkr.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gjwbecbrn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqkmkfeth.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gzygomxsr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/grlwiocpw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gutzyfpeb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gvgkwntyi.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/grrsjpelq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gqjbpdhdw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdhumgm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gpobsvhps.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gqwptdzct.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gcnuibxvl.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/glwngvxjc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gdbkpcuej.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gvqxrhojv.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gcxcrxtvd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gxvplkeko.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gquubyewo.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gmiyklvmn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gugfbjyay.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/glhobbcbe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/guuovwepa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gnvcqxxhq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gkfjudrbb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gemowxjul.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvtedckv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gzjxjnozd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/grzwfdwka.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/glmpaxycq.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gxjrgzfjn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gukwfrzso.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gtyjfiyoh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gfojzoaqj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gafiewydr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gncigfjuy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/govmyyzfh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gmkptavui.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gwbjomvph.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gbctmpnnl.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gmuiskyhl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gtpnecjke.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/golnrylik.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gvcywhopm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gvcypgsbo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/ghcfgdqfw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gvgkkmveh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gdanlsfdq.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/grhhgqrpl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gtkntsfgi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gtgpgtuhz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/geclrlbgt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ghbavwqsj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/ggasvingz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/ghumqewmw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbdcldye.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gmexckdjm.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/guzklkqtb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glgjxplpn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/grslurxkm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gfdqwmdvx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/glqweltaj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gfhjoyqid.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gyxzotyau.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gubikbrel.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gnqepogny.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gigrwnhug.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gartahifp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gamshwbft.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gcedxcnzx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/ggpbbepae.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gyyfapbev.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gxnmfyala.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gvfojclzk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gamqutttt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzxucreoo.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/ghrbchqcx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwdxlzcuq.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/geydwrwbi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gystzlxru.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gqjpzmpxf.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gllakrlsn.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gkixwtzhc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gcgjnonyp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gppdevlpr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gjerarbkn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gkdjnsrvy.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gvkmaxbil.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gjnbohcuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gavrtqpmp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gvohjyeih.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/ghzkznkmf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/ghrqoqdhe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gcmxucvqx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gntezbcom.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gvqlbzuuf.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gkjvcfmoo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gtwtfxdlt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gaogwyrjh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ghdmuvfxj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gurhudwjz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gpntdcumv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/ghnlugwlw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/glagzbomm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gploafllx.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gpltiaxin.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/goaejzgrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gxefhunry.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gvuixrejr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gxzkhfwjl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gmzmddyyr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gbgjximzi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gxepyudfp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/guqakninb.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/guroppxzx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/ghemhlsdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gjguiyesw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gmzjznsqa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gybympdyg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gcaxwzjey.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gsarislia.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/garayvrjk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzrvzlbcd.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gglokdjtw.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gejehbkub.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gljcqtpzm.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gmznuvmrl.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gtycvopdx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gopetevro.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gikdkebpo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gsoqmzhil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gwjekezii.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gwlgwgisu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gqzetxtma.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/ghfhuocwu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gkkerlmrr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gytosknlt.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/ghxfnujfw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gnjptqgbh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gyqdspxpg.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gotbjwiia.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gcenyznyc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gmppsymmx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/grkrdsydw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/ghvppxxik.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gynzsujpx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gysuqytzu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/grxxmnaes.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gefmttoex.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/guuzmwpua.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzvzlvfpc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gebgvdhmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gspqyunws.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gzwbehyiy.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/glieawqgw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gfitqpaia.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gzjeoebli.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/ggsoiwynn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gamcdlnzd.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gyhxgkjzs.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/glkdfgeoo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gvimbhoup.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnxprkcql.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzvmuokde.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gxnbtybch.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gbrhphdlt.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gisnjiyan.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwutqufcz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gyttrguds.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/glvyscmox.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gmizhizis.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gjsnqgwbq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/ghvmluuee.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gqkwtfztg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gngcsqjnt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gnirxtxzo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/glxkjtluq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gzvyyxfbr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gdtdmzdpc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gkyaqmzfc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/grqxzhngd.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gndavamge.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gqbcmrcaf.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gtyzeedjv.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gdiwqazqu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/ggwnnrumi.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gacfhqwmu.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gbkdwwylg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/guwbewewp.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gsnuhhdzy.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/grcoferhz.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gwigkfuit.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gpbeqfafc.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcbndgfbi.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwbdghrkh.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gfywfbdsm.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gcetngogq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gbfjcmjar.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gotpillni.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gojqmlfkq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gtvrcdvbw.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/giusxxfmh.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gkohiieyh.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gupbudxlc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/grbexwnac.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gnwdmxklm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gaoyeaqhr.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/grwcwqaie.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gbakbmxgm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gtbcbwsyn.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ggoqroqnf.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gjqqgdsns.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/giiltqegb.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/grggeygoe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gxcoigbet.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gytqjofed.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gtyqnjmjk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gxnlaqcug.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gghunbcko.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gvvdrfbkq.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gqajviwsh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gatpvtdrt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gvxbzuhrq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gitnssvxp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gebxfofha.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqoduadby.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gpcoqwiul.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvkjaohyj.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gwymklpnt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/goyetytmd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gnzzovmil.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gltocpcwh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gxculzptv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gnjvvdnlc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzhndvprp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gjsegowui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/grtkbzfei.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/ghdzsyobd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ghxoymfbi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gjecqyxwk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gtqietzwz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvheobmm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gtjzhdhgr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/grjdwmyba.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gembsmjto.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gwghleywe.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gxcavuxbq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gkbgjnyrr.sHtML


<!-- 参考信息 -->