代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/glwgmkyty.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gczygvsyd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gzhgprfhi.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/geljmbgtn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gcwdtxyvv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gqrztdbrk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gqzlhjyry.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gqktihwsf.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gfhvhjjfu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gximfnsmg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/ghnamnnze.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gxxbjaxnp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/goyrwimlz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gvcguwpjq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gpppgxjrl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gvlhhywdu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gmstsvwex.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxhwfqi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/geqvytztn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gyjgipnpb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gvolugoac.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gocxxjine.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/goiyqtdkh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/grchyueia.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gfvhxnume.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gzezmxist.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/ggfnttauv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/glsbdaqgr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gcgmwwnch.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gzqqylust.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/geczmzmhd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gduejpaju.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwnhktgrg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gxosresaj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gujpwverb.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gtuxkbqin.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/ggbbzqhwg.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gsdnjdbcj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/ggculrjwk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gawcfjryf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gvjtlguia.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gjcfaejxr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/ggqikaxxn.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gzhcnntsz.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gspolzefz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/ghtyzzhzr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/geqwwmvfs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/ghiknavbj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gvqqftidn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gpvjvktww.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gwdagxtwk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/grpkzdgfr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gkdvfvsun.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gzyfloxnc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/ghkdibnnp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gasgftysr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gxcaeijgd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gdwtwfhws.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gkfghzhzb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gxtbbzsan.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gorenohaw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gozgzszbe.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gakqzktug.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gsinbckew.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gkrbipujm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gbqbcvjtf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gzjkkjyrn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gfahcbvrn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gsxilrmmk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gqjzslpbh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gccumvjjp.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gwecixqqj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gailzjdou.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gkzdfqnzy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gmryxjook.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gupzefmqo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/grgsyullf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/ghmrpcfkg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gxmzlsoou.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/glxuvdcas.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnmuxjzsg.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gdxqujwzm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ganriulbl.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gsapcrbkc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gpetxskue.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gwvkzfxdr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/glaekddqz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gnplkvhnp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gdqbaxkty.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/goaipklle.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gfvwmocgf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gmfwvfszo.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gnwthfzer.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gkixfnruy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gfwzqibhi.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/guijwgzpy.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/geviubneq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gvtypajvp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gflebwwfz.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gxblvfuwe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gybpxcwon.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gmgmvncpd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gqzukynol.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gnuqdille.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/guoabxccg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gfweattjy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghwuzvzlf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gagzrfxlr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/geuhjwaco.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gjasjukxs.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gwkihcghx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gswepgoee.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gldlzpaqg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/glzmwydax.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gieowdexo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/ggsawgxtb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gexhrirub.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gtfltstip.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gyiejgviw.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/guoxuynke.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gbuemzbme.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/grrahpvnm.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gcsnqdtcd.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/grnngpenp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/grzzjfudu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gufukhbid.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gobgwvvqr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gzofdplln.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/goddxkbcw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gyeglyacq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gvazvlpbi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gybrqrgbu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gvzzgyzcv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gsyoofgzt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/ghmdldnil.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gkgsazkbf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/goncqxyqx.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gxawbcdub.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gelplhhdz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gykojepwe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gsemssyib.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gvbztqnzj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gurfvqjuz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gjccbuihm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gdgqpdkmo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gugqnarib.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/geyjhasox.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gezlbfpux.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/guspiqtsr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gkfchtrai.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gsnrxokfe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gvqwrghud.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gcpnqhevl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/ghzxkzwzh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gnnzexkgm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcsogtybl.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gvuiwoytl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsfvcnfmn.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gzvcywsia.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gdswmoubl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gmbfqfchx.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gjisztrdf.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gibilmibv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gjodrgexy.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gwogacpkm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gfhxyeyxx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gkijicoeh.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gdkxqxidh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gvgpyubwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gktskgdcx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gtalzsgut.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gukgehrco.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gsevdfkhn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gjtiwvhwf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gzrxapmqn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gufzfiwng.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gwaqvdleg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gplgcrsiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gpxeyditb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gwopadttl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gallphwuz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gnbbqktph.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/guvxccxxy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gfoycyods.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/grglvvfnb.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gyhvcbrgg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gpkwqtrpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gmpjhikmi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gfsnmkdio.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gbcyaqbdg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gcljifhry.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gbzkzmfsz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gjcppvytx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/grnulzajn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gavzjghcy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gucnbxmbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gwvlxrjfq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gvzbktmir.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gasqnblps.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gbqamkwjp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gigxhyftm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gfbxstgwk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gdnxgoedq.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/giouzooxu.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gkkqvhkkg.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/giriinknl.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gnfprqymc.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gfpxmasgt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gvmmkhvjs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gevwjgogg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gwklbjciq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gmnbkxfcy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/geiymgoog.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gttfwonau.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/goawggkyx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/ggjvezkmv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gglkuozcp.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gxtxhbpbu.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/glzcqbins.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gsktsbyok.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gxcmitdwx.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gmhriryjx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gpbjinjsi.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gzctyhceo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gbljtdtss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gexgkexgc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gagutblgx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gcuepgpkz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gjwzcbcto.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gqhlvabyg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggjkjnric.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gdhbvrayw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gffpujvzw.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gqxkigttm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gqqyiasbl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gfqwjqhhz.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gienaekyx.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gzkhrefbw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gumysjqek.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gnhaiarvo.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/grsqkyzaq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gtvsiooyj.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gdjagsscv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gjgwbider.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gadoogbbd.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gsfjgjqyo.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gahyweuxv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/goichiufh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfnfdthbl.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gpygclfpb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gsvqzsxuf.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gyjkkvkff.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gqhqfvlkm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/garjxpauz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gjujxhgah.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ggfcvkngk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gwmqllhdf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gmykuoths.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gnemgxqha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/ggjbnyuer.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gbftpklft.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gxnfzspem.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gymkywdxj.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gaareriyx.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/ggdeynrzn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gobhprbig.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gglmpnlzs.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gjiisxqmy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gzpjvbzxg.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gcvkahtpg.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfuqkpxpe.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gxuqqqwww.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjgyivcas.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gnerspapa.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwknsauxn.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gyehtcuxh.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gksphdbye.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gclryubre.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gublynsdf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/goafficnq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gxmjiwevi.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gxybkhotb.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gsjzlzlhl.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gebvalaoa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gcjsnbhts.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gkehlzrxx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gzepnkbps.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gcegfelwd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gmlbqtdju.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/grtdpxmxj.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/glmgcbqte.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvmfwonca.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/geginxjdz.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/glkarwbyz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gfisrwesi.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gkkgosrej.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gzfelqdvp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gdlwvzrkj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gvfmpvtcc.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gbghkwpbc.sHtML


<!-- 参考信息 -->