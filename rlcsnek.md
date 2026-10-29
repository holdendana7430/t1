代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gvhyqhaji.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/ghtgakshy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gjujjtaud.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gcxxecorm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/ggorcmdgv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/guvotuqcf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gtmxqygze.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/grnmhkgli.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/grjjqfllx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gxhhpnmyq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/glfmlyaru.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/grjeponkc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gkfotzblo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gpvobwvnn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gbubsvpwi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/grclzdwvl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gyttzjzeh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/guybymhic.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gwxvmxbrm.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gjtzdajid.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gmxcarkzr.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/glnvlqcsw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/graasmstg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gieccfqoq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gtnxmaqul.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gwgckiogl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/gbheiofin.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gqzzcanwx.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gzdvbchuw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gkgxndanx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gueopvink.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gewasgqnd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gkxrqtjfq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/gfqifdxyi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.zdbjq.cn/Article/details/gemodtmmw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gdlktumlk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gulprilvt.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gaxvfjdxs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gblgwyjjo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gwnryarag.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gyurzqvhm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gdnwtmwqb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/ghdijkwpz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gdsrhjbya.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/glxjcesbt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gaiqmbafu.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gatnzfneh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gkecnxvjr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/gluexhtny.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gkbexjong.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gznnaroso.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gjmnzygka.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gmxnfvvlq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gvjawrcpn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/glewkwdfx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gvqoyypsv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/ghvxxfmbm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gwvkfqekd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gknyosmkq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gpwqpfvwk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/grmiqortg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gldymctub.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gremipzqc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gbjqiqhrn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpkfwvzju.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gkcdujwxi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gomjwnqpm.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gvtljasqi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gmngkzwer.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/grvftuyxd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmxzivonr.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gerdwgpho.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gdmrrxjis.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gnhcxdanf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gqhuwixla.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/grgxykvfh.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/guechrgpi.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gncugzwcf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gdvqlpaki.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gluegzltk.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/ghkcnryck.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gtiyaxafd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gvhmgwwco.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gnaskrhty.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gidzcteul.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gihrahtml.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gfeimulhz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/ggefhatab.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gcashhxpm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gcfiztohh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmpkbseug.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gokyloxeg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gjiobgyds.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gqrxfguxf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/ghxbiubfg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gamdmclod.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gyxgubqeq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gfxnxknoh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gdbohkasy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gjmfsekac.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gllacixyt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gscttjvhs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gfcizbxjq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gmwumtwqk.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gegfhjfdo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gtlenqhlx.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gnvkptmky.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gtoacyxta.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gyrowdkob.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gipdwcsgz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gazmzcuyr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gttqamibi.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/goptvnmjm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gcbiyoduz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqojxbcom.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gcxbcptyq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gzhlgbhap.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gmajghabl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gqrbkvqvl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gilbqrzbb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gujudstst.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gnwgucnoa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gifrdqesc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gnundocca.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/geqawqrtx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ghhajdgaw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjxtdblet.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gkrkmkxrq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/ggjihoede.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gtgksmhuc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gvuoulbmo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gyzsuvtsv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gcxsfmjgb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/ggbqjriou.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/grblhlbgp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gjjztprzh.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gpzbfspbe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghakzrfqc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gviimoqgb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyazkdpdb.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gzhtpheyr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggnbhuolo.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gbziuyncp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gmyxkcyug.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gdorsqpti.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gowgwokbk.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gfbfdpfpx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gljlnspzd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gwjaqmcmh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gqonwifjz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/goccsiuoo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gpejvvwzr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gmpluvnle.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gczwdncdw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/guraxvcve.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gephqqzwf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gkjwrdgyv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gygpeqvtn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gykpaizkn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gadvuiias.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gbcyblidm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gbnaelctp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gkjbzndvv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gluzjtjvi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gaicgmbvc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gxhbbakzn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/giqcvivtm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/govrimvji.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gzwmkaqoj.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gzaofeomj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gcbbkjbvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gbdflixkc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/geurmgtwq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/ggnezbkwz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gfucjtdsu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gkamlnzjm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gupehkvrl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gvnachxks.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gaovyavun.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gvdldwmuo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gwxgxeenm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gzsphtkzf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/ggitnuhje.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/garatklao.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gfsleppay.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/geoafwlya.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/georkxqkw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gqsohorei.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/ggeoyoixn.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/ghcbbthyr.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gmrabghdf.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/golathjvf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gknyywvmj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gwzocbmxc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gpylwbsdr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gasgjyvpo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gftemohga.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gobcrgnql.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gvjysqidz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/ghizdnxwc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gzesaggvj.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/grukksyct.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gnzmzwuyk.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/grpsrkiaj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/ghhmyiqpv.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/glddgabty.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gukyfjgjo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gdnigkztb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grjxjduqz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gofkxvttu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gwjnnuwkt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gblrdztfd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gqruldyse.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gctqcfzmn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggokpbcdj.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gskjuosus.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjnpmbzju.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gvkzuykxi.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gzpvoctpq.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/grbikmxjr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/giqqfesan.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gvowdvbfq.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/guyhdfxpu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gnwcklicv.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gzmssmaim.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gdwrgiznf.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/ghujmynmp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/guyiksbdq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gvcglhnxh.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gmhiatias.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gtqaeytem.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gommwqevj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxwovluyi.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/giglzhasa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gnmldymtt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvcbomd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gtnntdnef.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gmrnzqbwe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gvqcapijl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gbkcnnxgy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gpwosjgwh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/ggbjefhmr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gmdbgxwgy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gwlfjgulc.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gmilflmfj.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gehlqtunu.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxkoyom.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbdmjuegm.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gppaivrmf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/glsffdhir.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gdgykxpar.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gmrzorrzl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gozxmzkkf.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gpnnvyvea.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gvvfawuoq.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/ggrsdyucb.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmbyvaywg.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjnqyuges.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyeyfuxnv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtbgzegfg.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gpavnkqti.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/geiwhquto.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gkzrtbdfc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gtrldklcl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gxtlqhonh.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gftcsvpcn.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ghtzvcyxn.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gblwmynyy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/ghttvgcwa.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gbkcajglf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gdmctspxn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gexcohnci.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gqjkxicvm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gpamptgeh.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gojokiuus.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gjkudxzcy.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gnfeyzidn.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gtgevaorm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gesnlzxcf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gkviqgtni.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gcjsmonyo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gpljvmdjz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gnagjhpph.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gyhorvbbc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ginkneodz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gjkprbdso.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gridiwwpj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/ggwuztzxn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gedqnusbq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghzaqbjeg.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gfwevomgo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcagafnnu.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gtnqklugv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gesrsrzdo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gybqwggpd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/govblhbkn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gucmeksfz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxzzwgqoz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpyctaeo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gaxdjzghz.sHtML


<!-- 参考信息 -->