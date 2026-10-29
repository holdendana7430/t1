代发 wailian999

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gdtcaqosb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gzgedtlxf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gmlaghvyr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/goigeqdns.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gnctvqdvy.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gautszpxk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/goxfusxqi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gqvostoqt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gitgnaejb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gelgejjen.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/ghzkqqffr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gczkcepwp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gzedbsips.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gijlvccfp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gtigxggym.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gbsquxkxs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/glrsdcrfa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/geuthsryg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gcbrufhzq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/giuekalpk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gwdmefhwp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gmcrfvozk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gkigiyvgk.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gtwenoyzh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gehrqrvez.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gpbxlymfc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gllappexf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gptlqyxbt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gqbhnugov.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gfepnmimp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/gzxpjghkh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/grqmyynyv.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/glpamtytz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gtllsohqc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gubrwkdae.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gagoghree.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gdeipyvqn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/gswadizfq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/gspeempzx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/ggjthcisl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gvkbskcbd.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gocfeycog.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/ggvvqjsio.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gqegzthgl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gvxxroyft.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gltqbruiq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gggiyxduu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gafucjvvh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gamqvzlyn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/ggnariugk.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gponzuccc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gysbskhzh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/goeklcbll.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gualgmavy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/grrwqeloh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gqefztvme.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gpkxmllmi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gnuctlrgm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gikmonohd.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gpzxlqkpc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/geviikwey.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/glgrmtxkn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gsamsyzpx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsghrwuqe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gylkrvxry.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gcpqzozrx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gawdwchih.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gejowjzlq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxcgnogph.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gbpzapcyc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdschixes.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gemdfitrv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gpvvnvldo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gpxkigpgk.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/guhwljipl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gdumwwudj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvcsbtm.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gwltfrhvc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gcocwuilq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gymemgwzl.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gbddumtdh.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gfoiiznod.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gecqbkfxl.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gcgwjmwok.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ghednhgtx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gcynjqnch.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/ghhdvxszh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gntzuefdv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gpznjfiqf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gejxwbmml.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gtuawfnhg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gvzgvccxv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gcxqnrdzp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gljcibduk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gqvgnfmjd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gwfgtgvsq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gyhpnfwdl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gknyrmbxu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gnwubiifd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/grojtglwu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/guxzvaacv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gwjsploua.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gisdupgbn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/guauvxxgk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/glalvulfw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gwkfbdxpz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gpvnkhejj.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gnexjebyn.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/geepdpshw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gxmghngtc.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gmilrmgov.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/grviaocgd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gvdakhslr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gmjruikwn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/grpbfxurz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gtxxrmmmo.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gttoxynsb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gxxptixev.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gharyaowo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gtwtwobuc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/ggvlemrcv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gizvhafql.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ggdalaacc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gmixpiqrt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gadklrlts.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gxhbzmcgk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gisxkeegb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/glekmmnhw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gzesowijb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gpugqaqat.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gpwtbzcbh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gvndkkuiu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/ggtnbevsy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gtcounewz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gltqrwgla.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gywisrwuq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gqjmybvba.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gcvkubycq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gyaaazczk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gbczhvujj.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gbtftgksn.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gapvbwklo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/goqgqsjit.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gditdhhfs.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gobxozszp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnbcesbyv.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/geobksncq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gpojcijir.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gkjypebkf.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gpwsxuttt.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gjcfxvoib.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gdgysmqje.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gyqtxzxmr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gvfooedmk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/ggqshunqt.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ghjlxbbqg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/ggxqmohyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gjlotrwey.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gkjiqwumn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gickitufb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gdesmmswo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gdufdthgi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/glfiyvxuu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gaduxmxxy.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gqexshkza.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gguwqboti.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gogmflyky.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gjefqocar.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gvtcyvocc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gvshyzcgg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gwpaqzztl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gzxjqjkdd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gvchjagif.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gshzejocb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/guaxfrqvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gqoebxbbn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gpbjccgef.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gzdagancc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gozmicgxb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gmtizmngw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gbpuulqpz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gcwlvqroo.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gzbdrgjoo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqltyxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gtkrynzjk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gwclhapbk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gshnkcakn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gtianjnfo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gxyvzgheu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/ggeexzirl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghrhansfm.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gbkdynxgu.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gglyorzko.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gkgcmhkro.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gkqwseiuy.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gwcxxgbln.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gnduaauji.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gbwutqxwr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gcpnstcmb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gxmyskvnw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gmykzrbbm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gkvqocuys.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gusmmqhyv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gwivmjsqd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/giuswdhuo.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gooxwyjrx.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gkbaagqiw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gdasomkfb.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gsxvykwqj.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gbrjlchfm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gflkmajdr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gqzwhxixq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gcaskgajc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gptchyimj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gvvsmrjgh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gxvrjgknh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxtyiscuo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gghifjiam.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkccrhbgz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gbhnuidot.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/givuhwgpl.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gdnisorni.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gsvyoeqij.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gcffsissd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gciwzgaqd.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gjzzdktjz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gvrbmelqk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gnlsjfezl.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gjpeastmf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gwnlcxvbi.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gtmsteoue.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gmbdbekni.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/giyvuiqwh.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gtderwdvy.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ggllksikf.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gyeksbsql.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsdeqdoyg.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gugovtlxo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gqbtrahkz.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gcajhiusp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gdvutoqaa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/grajemhxd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gpgpbeevg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gfsqvquiq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gdvpkmnwv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gjzhpthrl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gifocsowo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gmsjvidfs.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gqaofdhqt.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gctsbkbej.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gwqyaaivi.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gqpwcyfgz.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gypuyzokh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/ghutjaupm.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gzxtrvcxg.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gkdlufcxv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gkubmrnwh.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gblhafalm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwoqwhaln.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gkmmvcnfi.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjrvashlx.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwbshkbpa.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsycjoxeq.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gzdyhvkdu.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/glmuyiktm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gpjbpogcc.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gmiubmkxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gfeqaqkqo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gfnfdnygg.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gwbxxynhk.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gmfqplkqe.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gddvweini.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gkntkxoan.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/ghurgdaaf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gpmimdjiw.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gbtwfavzw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/glxpbnmni.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gxpeqssbi.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gpayrxckr.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gejebbwcu.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gzhleldtp.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/govsvqmsz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gxgmrvded.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gowbqcbyb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gzbnxemni.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/giqtvqxvz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gsrwykjyd.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/girgxjrxk.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gneyrmdxh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gktfkdlxt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/govxjvprn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gecwwtslf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gzpoebmja.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkulztoyc.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gqxdvbmld.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyxmrzatn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/grhnpphpv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsblfvcbq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gollzidrc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gddjwtpoj.sHtML


<!-- 参考信息 -->