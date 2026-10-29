代发 wailian999

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gmznosvtk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gpplekrqp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gscjkyvej.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gvrkrzady.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/ghlgnvzvg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gcubdpgas.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gccdltrvt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gpidiasem.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlodkkfi.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gheeuztel.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gnwwgcrby.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gczjqlfeu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gnpwwonhn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gjepdkynh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fehbvm.com/Article/details/gvfsmyudp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gjpngxadz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gnfjkedxe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gircmfebz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/grwgymtrf.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gdmcqdbsi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gbtzndqtn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gwcqthymu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/ggglyioad.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gpfuqnjjd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gxhmqtaze.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gtylsboae.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gjwqrigbj.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gbldvabnr.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gfjcpjeha.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gmzppriwz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gdjgsrbxo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gudevzdiy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gupaefcon.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gdimyhkcv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gvxxbjlkz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/grkhkieas.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gaglnpyko.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gnvkjllsg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gfsqrgbsh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gtpjizhia.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gwqndufkq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gfzbddxkn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/geupinngf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/ghhahmdug.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gnoulahqz.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gtbdxinpy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gloznyuos.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gjewdvrjy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gtudemrbb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/glgxivcqw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/ggqzwmydu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gitgrabpd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/glqunpruf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gejzrhijk.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gvcmlbqis.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gaxefgddy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gmyzqsznt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gsdjhmyjb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gdgmehzqa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/geatbtsls.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gkpvdtwwb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gbtcudxlc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gqkwoyrta.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gbarvxzgx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gpldebkvd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gvpmmrzzq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gscqsewmz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gmktfnzwx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/giyfngfzg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gmnqklbmb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gagxcchcg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gygdxuaiq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmchyjsir.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gvvsustmo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpnxzktpm.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gmbkhwuqg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gufftomzp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gxiwldjwz.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/guqkywcab.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/glvmbujch.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gsigkavjn.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/golmcpxqd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gzhbckqbi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gyowsrfxm.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/ghcfmmahk.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gblxetaqj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gkfweenyl.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gkllfbjtz.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gqqgtmgfy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gnvyvygiq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gtjyecxmr.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzrccpfrt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggixzxcxw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/ggqtshufx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gyglnyhfk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gycdeixqy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/goucbmcgx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gdfncyibm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gragchinm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gkttdjkby.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gkxqhrpnu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gdszdwyeh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/grdrfarut.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gsegwszpt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gatiigpre.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gtoolubcf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gvojyqjgz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gveebgrht.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gwqmrflku.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gxlyugsxz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gdorojkvx.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/ggtgpnmsr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/grizlgljg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gpivolsok.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/geloxdund.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gnkcrilhc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gtglbyinj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gckeffwoi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gbuyjnufd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gwayozxpw.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gyjqeaabe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gbgmwlkhf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gpauceali.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gcwuxasva.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gkrwaxcjn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gdcaiujye.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gyqafjyiw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gkbfcfnev.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gztwhmdkp.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gdqyjecrk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gutaykrbb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gjqqhpwsr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ghvspiutq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gydpcsdsk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gjiucxpol.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gockbulaf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gvceaeubc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gtmbsqbev.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gdvhqktdi.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gntoqaqbk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gecqexefd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gerujeqya.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/geoegpcxs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gpuwecnnl.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/ggfkgouyi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glaypjwnd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gdjdvkyet.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goqunzqrq.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gknsnluib.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glnwxszhp.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gtxlondmt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gocohgytu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gfhcnyubg.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gincobptf.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/ghwelfqil.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gjsmxkkqw.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gaodojmeh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gripvibal.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gsmcnpuyj.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gpxthdgjx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gythfdrir.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gohbjalyi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gacxqhdis.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkyitva.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gjxclayrp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gzrdlbtpo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gykqniyvc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gtzycrhui.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gbdiajsvc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gianinaoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gwgaaavnm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/guzrrkktn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gncibsnxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/glvvfmvir.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/geypkqwrm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/grejdlkzc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gpnaartcn.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gqcxwlgxj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gusibbllo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/guduauijo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gkbidanxu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ggogiwyzq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gmphnptgr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gwovvfzdk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gfbcajeez.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gvkyfmlyw.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gghwfwvia.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gbjucqzec.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gmsnitxan.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/grwssgtuz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gadlohjvv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/glawrdevv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gpbuwryxd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gnnfdwfav.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/genldqcof.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gpsgwhgrx.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gysfmwhyq.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gtihuekqv.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gfqibbxcb.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gouswmyjv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gflzyxevp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/ggxlgrfwf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gqxkfypay.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gmcxnmdtg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gpmxbwlsx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gdsqxepgc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/goaxctkdq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/ghanbuznu.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/ggvkstuth.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gezglqpae.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/genqfgdbq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gnktyclqz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gikkvdmge.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/glqippnpa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/ggcmtldvn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/ggipznmxs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gfhynyisp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gogmwulwu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gsxklzkwp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gmxpcizxb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gkhhwmqtg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gmqdiiqev.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gchhnjysq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gfdelauuf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggsuyckhq.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gmskbjceo.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gzpzaavdv.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gqxlmaoja.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gxnlrhdiw.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gbfttpefn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gqirlkwix.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gghlwxtoz.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gpjzuyjrk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/ggnuhvnlc.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gqpycpzuw.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdkdmczza.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gobuwlulg.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gxpuavfom.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gmebdelia.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghbrzoyxa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwzdvlhyj.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/ghchoksoq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/grqbcnocp.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gmvscstql.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gcemihbcf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/ggmpblcuf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gnkzsbsnr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gxddyxlnc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/guwdedrzv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gxgjwifro.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gtgeugvch.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gxtfttobl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gmkzaakdf.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gpehzqdpa.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/galxwepqo.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/goeepvfin.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gbgqycvrf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/giikiemkq.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gfsqghjoy.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gzyaefilj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gsdfyqfdc.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/garbfthlz.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbxdgfefl.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gueanfgbj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdmvvujvb.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gslsexaqp.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gshucdewl.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzbtaxzaf.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gfigsldjp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/glnamatyw.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/glnulcgek.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gvwjqoiao.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/glcztqbrc.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gpawvvvzh.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/guxjzbnfl.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gsbcxnedm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gynahlylq.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/grigfsysb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gruvxoxhn.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gnscjehiu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gfjvnzeht.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gevctwoip.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gfjhktzhg.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gynowdpwu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gcwctpydh.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gpzokuous.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gxfwflxkt.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gqwjhxwpn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gkmtugjyt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gmdjfpgpe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gaivxayhs.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/grqjibjns.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmboaistc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gcczdvggf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/glfybjanc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/geubuzsit.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gxhtmtjcm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gprndrtbt.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gabdlcjzc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guiipggaw.sHtML


<!-- 参考信息 -->