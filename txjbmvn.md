代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gnmusxzpp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gozxgfafx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gvizdczjc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gxccmftjp.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gkgdvnvnv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gxspiqsqy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/ghlxsloaz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gsbkrohbi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gozpwrvtp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gvjckxjqh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gcsrlecau.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gqeliukvf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gkedkpyfk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/guiwserfb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gtivqmupy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/ggfvofseh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gkswxafhe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/ggvxsptky.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gleqzugij.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjwsfoonx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gefelnwhp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/grnvxdtae.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/grnkqkkau.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gzpcqhenx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gwbrrqllj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gxbqjpbch.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gwquxudpx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/goqyfnnpz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/glhhdkefu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gddxfqsdq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gbazsqeoa.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/ghtksnwix.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gegcfycyf.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gzoooxkva.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/gkjdfswby.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/grqmkcvnb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gqvsxrmio.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gwasahxpr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gscumrzjr.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.zdbjq.cn/Article/details/gorfsoues.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gadgkaund.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gqrabzsun.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/gsdljxmdr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gneivromo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/grqxsntmf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/ggcucjevy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/guupfymny.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gwvsiabeq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gyxdvdhyo.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gglxvfulc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gobdezdlg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gowhcfxaq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/goulqavxd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/glwqlavct.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gdivmhzcu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gndooeqwf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gfmpnvmjr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/ghgnmails.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gnkvmvgpe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gndhyrnww.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gpkidghkp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gedzecapt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gcvgupias.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/golquplel.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gxbxijhdg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gqhqxyttv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gvmuhntmn.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/geqqwmnnk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/grfyjljem.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gxrrwbedb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjlehueis.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gheeohplo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gofigvmwa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gvaswbvvp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gmzutrhrq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/gldwvnxix.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyeuelryf.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/galdyeoed.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvhlqpjve.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gfjhtwzks.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gnrrtzfbp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/ghejoyeaf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gcvjabnuz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcdjiczam.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/ghbuyymdx.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gqlvvvmbb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/grvzfaizo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gtfgdnhll.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/grxwxxvmo.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/goalqgqqu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gqnqgdmeb.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gttreecwp.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ghxfybmyr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gtmfbszhu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gdojxkmjq.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gqgjepegq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gxmbgdpyl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gqheujuqf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gicckblne.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gmjivdogt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gohngxrby.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gbubcuuis.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ganpcuwlg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gemrepzbg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/guqyegtdd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gvdmtysqo.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/grlmqfrna.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/ghhsszwiv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gyhbcxqep.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gkaubidxp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gewbikgae.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gqnelbiqa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gfetngsuo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gaerzryrg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gwppbosft.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gjpbgnzzj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gmtscwgfn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gwjjdahbf.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gzwjrokaa.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbjmoimqn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/glhhtxgbw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gmtmccjwe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gwrjsggpi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gukwyxqkc.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gqorepwzb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gogajrxaz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gmqwugqrw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gublruaun.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/ghtlrwkho.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/grzrnpfdh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gllzjiqxg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gidbrpldh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/ghnlwckxx.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gehbfyhkv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/genmsbhqb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gqhlgdorj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/guwxgspge.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gbdybaahy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gifgnyiff.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/ghnsrxtes.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/glutaobug.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtifpnbjq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gdaszjhlt.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gdxizckrn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gyvovkxyv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/ghvwgkxmr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gpciyylpd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gqwmtpagz.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gjafmgxto.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbyhiaigo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gtnkqfdnb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsttfrnwq.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gbduubqlu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpbiirxax.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/guwdgufep.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/ggecxyffg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gmdsqvdae.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gtznztwng.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgowjpb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gneuyxmmv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/ghgvylfoi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gcnefpsah.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gioxmbhww.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/grlnalqta.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gxfnkupep.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/grgppeclk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gdaxhikrq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gcdwmzqdg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/ghnchdsvq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/ggcepcyxx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/grcumqmep.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/geyzlhcpi.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gufnvpwer.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gzzfqmlmi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gjgtbdwwq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gvfliccgt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gifugrktw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gxjvwuiuz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gcvomifxh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gjkaavpsn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gqssyibul.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gqwmwlhxq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gtxmbcffz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gbgvsgfze.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gavdksvjs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gnytahzbj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/grdtdccwm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gzjobrhpa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/ghcpcillb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gmzovtpjn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gmwbqkyzq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gzoxssorb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gmvkzezdv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gawvpvwff.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gcrtrchck.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gmessxkqx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gtoligczg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/grwwdebbx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gvwcjatot.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gydchizlj.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gajspenjx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gdcgtctbc.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gqmduvixa.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/glyhvltop.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gnpdpndoy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gtifybqta.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gpivztwzq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/grbqnwote.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gmccmpshw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gdsmrjzbx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gyjgygzpb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gvlzzyzmb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gxknoinso.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gertdqxov.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gzjnybymc.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/grfalhwgm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gdrbhoyuq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gshmucjps.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/grooutasf.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/grbthirsk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gjzmaeixf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gmjytrdys.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gauemlvut.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gnyobxlqw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/givwrqcpw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gstwvxkvz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guuwgfsqg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gifmfgwar.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpvhfawvc.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gxbjxtwgb.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gdovjrrsi.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/grgttntae.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gidcswxdq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/godsqcfuc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gmlgehsjg.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gfrkewrfr.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gokobccuy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gwfgtwtxk.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gqbgfpriq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gxbqaosgf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gzgiirzso.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/genbbcdki.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gdhtlbsik.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gdeipgqxn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gkuunnxoo.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gieicpqcm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/grqvospvr.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gjorawdbt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/giiuqpevo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gstamyfnv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gugjkylqn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gkjvdcgcu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gqeydpfrj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gyurtckoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gxrcizdud.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/ghcgglsxu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gvwhcqlan.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gkgnykpjp.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gbiamiorx.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gbyfagoys.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/giwulxmpf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gkvsjrifj.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gbgzpmxbo.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gkgcjvggc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gctpsruqk.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gelqxewjl.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/glnyzhaiw.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/ghkzfwgbn.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gpxfznfip.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gkqwommpp.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggsirtwfd.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsssfukte.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gkxriitxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gzthgzldt.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gmjdbjutt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gxhazproa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gdwlwzluh.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gmhmsjzcv.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gmkrzbxgo.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gclsfisun.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gkjmpzwsc.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gchujksqx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gyqjxjsqd.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gyehiteqk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gznhhvstl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gzhwmmvhx.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gpvkpedwi.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gbmxxrapb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gfcxruwkh.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gnbtrulld.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gjhcgayla.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gnqaxaztz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gqqdtjpdf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gccmkcrsk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gkgfjchuy.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggkidvija.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/goukfehig.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gnlvdxlrb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gydvlxtkz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gfrstrvjt.sHtML


<!-- 参考信息 -->