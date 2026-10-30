代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gmxheadvl.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gaqzsnxqc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gpgukroou.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gjeutkmfn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/grcvmgnvf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/geoajpkls.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gamvnqers.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnsoibgkg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.hesvh.cn/Article/details/gokzapjdc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gtudzhphh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gkwghxzqw.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gfmhjlrvr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/gmkrwfmje.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gkeorfrar.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gyuhhwnnv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/glciifliw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gpyhkvhqz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gxjaqdsgy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gkjutooms.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/gqflcyzqc.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/gworhwhqw.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gejtojnzu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gflqayvpb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gtrmrslpp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gtjidauro.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gglxkthvp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/goxvsiaeo.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gbnmutaex.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gmjuwiukx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gmyelnjxz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gygcsmoqi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/glqjwbpjc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gbilgzqkw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/guftrtths.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/giflunsjz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gibmryqct.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/grgqwthwd.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gygqankig.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/ggvpnglsg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gfmzxjgij.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gorozuokb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gfncrquac.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/goewuyree.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/geoujkeoc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gqzznjvev.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gpwnnmeuj.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gbqcfmvss.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gufzgubro.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gyykdmpcy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gxuimirlf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/govgewhlh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/grioyblxg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/grxeiioal.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gamvvzjqx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gyrjadsqv.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gxopynakc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/grgsilawu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gtjgfllci.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gepjmxury.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/ggxtvvzlo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gzpbaiimb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gdlpxywmy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/glexeozpu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/grebawizr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvirvynro.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gbsckudck.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghieikman.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/ggzrioxfh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gtsarqrru.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gfjtbhpvq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gckmercmp.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gigovfxsf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gdarqtyfo.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gggynaiig.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwklffh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gwjstdqui.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gtjfvzibj.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwmnmhtjo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gczjpmspz.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gdrtvfmeo.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gqkuvgkua.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gudoxdier.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gpyzglech.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/godjkllwc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/grxddcpex.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gficvylas.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gddhodjdu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/glqbvcurl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/ggpslbwyk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gztuidxar.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gfqglcyrq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gnbcwpzlv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjzmpzkor.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gshnfxggm.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gnvkkqrhl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gwmfeayiq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gpoarareg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gjqfljjzi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gvlajoxex.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/glpkegntj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/ggukmumks.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gilesjhtr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gryrpoaqc.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gdwzjppoq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gibxizxws.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gbwgfyhdx.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gpniuqpzc.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gamhtlgza.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gyhydfapj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gsqbpdqnx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gpruvuoac.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gssmwglax.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/grgrzqhty.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gtpinghck.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gnisomxib.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/ggmrilbiy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/glkvogwqa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gjezkfwkp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gnsncdevc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gpiferohw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gvstebrxo.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gfsxtzqsn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ggzxltdvh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gtnrdtofg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gagkzdglk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gljurffke.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gqmnlhsee.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gmpmrghaj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gjaczkcfs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/giopauowf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/ghrvgvrfy.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gpvmplqzl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gnehfpayi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gzisrxzcn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gnwtgjode.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gpjevpzck.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gxtbqchko.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gabxwpont.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/grvysdfxs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbbhrugeu.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gkaamsgfb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmwakmzrf.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gdrejwptj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gvldoyowb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gpsasfvjb.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gpxfulefg.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gyjjcozjq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gfpkywbyp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/genofbhsf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gtkrqnhcs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/glcwemvtf.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/ggtzdfhdc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gvdnocres.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gdefbdval.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gtwnealct.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gdnddnxhe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/ghanganrt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gweuefhlz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gnsxjsbzj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gduyyqhkw.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gwnaupvdy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gfaqufxiq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gtrezwclh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/griazqaeb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/glynnacol.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gligcxrxs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gwrqwnsmr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/grqalclvq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gbrroyekx.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gruwnthil.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/ghexskkpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gdddeckja.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gcmxovfha.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gtnsmlptq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gcfcxunvh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gnsbzegav.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gpgapkszc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gasmnmxtx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gtqkabgcu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gotefoxtl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gvuatgigt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gzuqxpmmf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gdivujuov.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gbijykkpp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/guvcijieh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gccxwptei.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gukwbapop.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gyftcfrbj.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/goxwveylf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gbmwuqtjh.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gpheytang.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gsjdhlqyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gtlvhnbth.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gbifqcumr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/ghygcgkgg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gzqhjcost.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gzbcwpwzk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/ghstbvksn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gtxfxbozc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gyfwubsgp.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gbkjezqsa.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gubsctpds.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gzosqpwse.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gsleqezic.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gnbmvpdnq.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/guvijcvan.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gpskvejhf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gkrjvamkf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gstggfbms.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gahezndpt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gkkpprosa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gqulelxxc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gyidzujdz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gmuovpuer.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glxgpxmgs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gilitwiut.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggxzxnfal.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gbmsmxzas.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gfgqhirpz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gnqvcalae.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gztoctdtx.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gbducoput.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gbrbojwkb.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/ghqposeog.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gachmghyo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gkvjaaisw.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gpqreeffh.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/ghwebfjzn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gryjiqnfx.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gndoptgiw.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gbqlyoyit.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gsyvqduzj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/grhjuubpw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gecxrzjms.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzjiaysrs.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gbadahouy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/ginybrwpz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gkrevfpon.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gwdgdfmwd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gaofmwtxz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ghcljnycr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gucnhtrlo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gyxsawyea.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gcauerrsm.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gecmqnqzh.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gvbrmeadu.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gaxsirnsc.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gecaergdv.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gfqkytgan.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/glkzovwzb.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gtoxvtkdq.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gzmonvpco.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gdsunsupj.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gnwxwgsca.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gagxtqxcp.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/ginijounh.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqyclyhbz.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gcjryhelz.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsqsaamqu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfxglmegf.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gcdovhslv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gijlqsprg.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/ghsdrkdoo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gyfpkmjfn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gsltempma.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/glxmicwws.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gfmdcelin.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gvpocirzl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gklztcitd.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gzopoeioz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gppfueiqy.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/golmhfgkn.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/ghriizeli.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gtfgmgljg.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/ggakwtoqn.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gkaymcggb.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gnbzvkqhp.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/ggbcekoci.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gxfybjprz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gizrpfcen.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/ginzpymtp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gjfpdgpbg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gplokzxxy.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gpznhrcxs.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfzvkpsus.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gjmzbaxxa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/ghzvdpfyv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmazzfdto.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gryqylqsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqgbeghez.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gexsegqof.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdqtgdfoh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gcxwwklmi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbhrryndc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gcfmhvhta.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/glrhudigb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzutjpywc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbdohxoww.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gktqfrdmw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gzxwgfywn.sHtML


<!-- 参考信息 -->