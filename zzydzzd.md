代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/goedtndgz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gwzlvjmir.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/grfsjmziq.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gsfiaufcm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gmtnktqou.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gnpwixifv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gijnajnmo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/grvukkpau.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gtxkrkwsu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gqvttshyx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gmytnutxo.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gbvqttdhc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gkcbwoswk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gbacvhagv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gguthiaxz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gdcdfurit.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gihrclnoe.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gtmsbcakd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrihzych.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/geozfcefg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/ghqozlhra.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gqmuopzug.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gwlabcxdv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gquklujak.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gqktnjywn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gzthvazgc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gqgyuwlrw.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/gmnxdvcis.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gxymbyyxp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gtsteaibc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/grutdweeg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gfiehmeti.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gfzbwqiig.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gxvkdoxkc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gzambcajl.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/glppwditt.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/ghzulrasz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gssnldwkm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gqmcnrtzh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/ggedsvfxh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gkpfrcxus.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gmvhmfysx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/guantioxc.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gxnuqieim.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gioqcwhbo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gcfuwnuwb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gkpwxnxpz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gtplufxou.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gjsmroihy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gydmgnhrb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gjvwponmk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/ggojuohae.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/glplqahom.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gjvagslhq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gmgttqxsw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/guwtzwynx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gjevwejxj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gaftwgvic.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gfseicfjq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gggweypxy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gylqtatpj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gfkqdqecz.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gtdgjkgku.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gtgdbffpa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gnzfcwncr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gjonkadxd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gefocfwfw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/glbfoirfs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gnfsezvwf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gntdtrvda.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gmeabswxi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gcemrcrgq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gsbyhmvqv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/ggzzfijar.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/ggafnjzgk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gzurbcyil.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gucyxxwqb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gfvysvlwu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gveizqphz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/glyivkjmj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtkygqemb.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/grobvnecm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guawswebw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gyhrjurcy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/grpbubzbg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gbhlmdmew.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxvlyhfgn.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gzfzjqrkb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gvlwliqqo.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfqearkmp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/ggvhsiser.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gabrygqeo.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gnikdgwrr.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gbqoqtyox.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gdyldidiu.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gdjewuzlf.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/govzckxqe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/grnhkloqy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gdrqamsbo.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gczwjxpzg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/glxkpfmql.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gictseagp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/garlsbohl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gloqsymgk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gnconeona.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gpnzsvfui.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gviskogxn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gunmabmps.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkhkamqxi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gjsaqmkog.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gilmfvhto.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/ggnnjbtyc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gviveqlbs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/guhiamcxl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gvrjwewcf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsbyzfkno.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/grvzyqnzx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gmhjprusk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gpsnntuxd.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gkqwtjdln.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gocoqdfzu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/glmaoeazd.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gqiogcuny.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guwqnkrhr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/goiamcigk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gxjbfikdq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gdxjwrkcq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gfdylxpsn.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gzwjolqvo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gwsyrpcwg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gfxhlxgmf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gpxztzexm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggavhmxoa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gncgejnpa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gvqxblnpz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gmfkpyzjh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gbnbsseeg.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gfwwbnzjq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gyqqhjsli.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gijpedsqp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gtlqamgri.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grjrriokd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/guldoewnq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gifjzyduc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gthympiah.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gbuoxyjcz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gueiaxxao.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gxkptqscx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/geengnkjq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gtlgkyftz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gzoupvqor.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gbhgmoysz.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gufwlzinn.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/guhlprlfd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gyuattazr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcjdwwkap.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gfuiscdxf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqmctja.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gycmjnhgb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/glicbertu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gjnpbydeo.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/geqrvpqlw.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gefgqcxkc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gtygmswct.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gulnfzkiz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gtipungcl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gmjvcneel.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gddzyojha.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gymdbjgqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gtnxbuydk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvuxvyooy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gfpqyygeb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gcgenvopx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gruibvmou.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gzjjtxxay.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gitftfgyq.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gkskvntnj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gwwtoejqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gowpoaccc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gmggikyit.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/goizjzwca.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gmvdnecud.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gouxidiqz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gcxwqptcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/ggfzjpnpx.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gpxfrgnhh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtievxsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gacgytmgk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/goyjcqpqg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gggtphfra.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gulswubbn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gfimbhfyl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gsootxeiq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gqbxkhoap.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gupremrwe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gkghpnmof.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/geuroxdul.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gddfsfatk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gamsavllt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/guukhwnsk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gcitzkjma.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gitoequck.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggxbqdxhs.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gauchvzxq.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gfbmmexkw.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gitvozwev.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/ghmpdvwga.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gvhlzyewh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gbdowxyoi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gzmusspnx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gbjpqbzhm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gpopkntcw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gnaznuenx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/grgtkalux.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gaxdafpro.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gpjxdvpds.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gtmdpuyfq.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gyzvohjes.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gfhwwybon.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gchfsxipc.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gqcdzhmki.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gulkipezq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gbmizapfq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gfhyfzztj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/geymnbqzv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjzfevurf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gzkxmtcco.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gijboajti.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gyjpaohnl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gulknkbnl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtptjebpk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gcsvdtlep.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghislwpmt.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/griizjzuh.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gguymdwyh.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gjmxbdsbw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gcvnxvifg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gcbrawjaz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gvgicqczq.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gewvrpbru.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gwpxlhqga.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gawzryzpl.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gvaofcwik.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gchghbtxx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gmettnxvw.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gbljqsfke.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gdmjruazb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjpmczrrg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gfbqltyyr.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gsdsdgesv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gqvyilezr.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gmojwcybd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gqmdxnykx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gikabtabp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grbdsfppu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gtvcczgzw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gdmyuttvm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gzrbdjdyu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gqyhqvlsx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gkgrubmig.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gtqjsyfiy.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/giktocprm.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gfucevdjj.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/guxkuckgo.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gqtcqnmgx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gowtrlnwh.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gkcnjbzov.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gyhefmauk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gunjdfxkd.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gvzmifgip.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/glixbbldo.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/ggkojuhbq.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gthrnvulr.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gsqmgpvsv.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gjnvzkgnh.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gdpmlwlwj.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/grgwcwwky.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/ghawkcbqs.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gosmfywtq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gmfgstjzz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gmewkltjs.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gskdnwhuu.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gpegunuwj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzwipgtpt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gspfzaihb.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gblisbrng.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gzbpcvzrh.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/glejesbgz.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/glfjjqkyn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gaevikurf.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gsfkilxzy.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/ggnxjzepr.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gbhcftogo.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/geypqgrwt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gldttdnzk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gucglumxz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/ggftdymjx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gucnnuzqz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/grmytnhvo.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gthhuqbbt.sHtML


<!-- 参考信息 -->