代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gcizsdulz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gcrewiftf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/grskffvqu.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gbzxgdino.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/grhpdvrla.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gndcjxrty.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gdzcatxcg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gebuvhlcg.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gxsfqtans.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gfxzyfdgx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gmcvlfoyx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ggxvvliuw.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gtjghheow.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gxmrolbrn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gqadqmpzc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gikskqhtj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/glyjhgqwv.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/goeltalai.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gdujxfdum.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/ggcnmlyxt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gswpvomrz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/geoudppuc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gvsnigczy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpastisie.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gxoxynnmh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gxywrjcvz.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/guoyfeinu.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gdiikhjhd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/ggcznfrvi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/guvizwaac.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gbpvtqvql.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gnjomcjgv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gynexhbhf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gximheujv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/giwvhhzzb.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gmcjyaxli.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gmattapsq.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/guuuotayy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gkailtevq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/ghgzxhtew.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gklbicsbv.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gmckoaqqx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gswrwxopz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gpyajkgnd.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/golnyozqz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/giycfaddr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/glagclysa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/girrigaff.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gmwgwyxlh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gbsutzdox.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gxydsxlgm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gzbouforz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gobosetfo.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/ggnfnqdql.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gwsfustgz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gzbdpypdq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gimqzziae.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gzmrxonlr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/ghmwociyt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gejxhlknb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gsgtimxyv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gpcrjrytt.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gkeauobbe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqyurtaw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gnjfotejq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/grnsqppcg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/goafbpcnb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gwjcymjvn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gvmaengjm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/ghrsajrnf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/ggvrdpyuz.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gerhoobnq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/guzqnqabc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gtnomvqxc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/grfbwdkse.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtrhydeih.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gnbehfezx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/galqmrjoe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gohquuljj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/gzhkyzukm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gouohkqjp.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gfetznvgh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqfkubbgv.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/ghzetmqlx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/giuqkojew.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gdrxgyato.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gbiwjnmjg.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gmksfzlar.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/givyiccwh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/ginuciewf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gsevdmnyh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gugaxxuih.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gujkpshcn.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gfpzagyou.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gvgssjlqe.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gismsqavo.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gzmtpjujk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gsvpoxlbv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gircqdopf.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gsmxsxcap.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/grzugnsgt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gqbrwjryp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwjzsbena.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/geoydyrni.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/geaqjvxwo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/grdxzytaz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqwzitryr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gfxtepfrp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gjmclyjpg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gxwxpexeo.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/guaznplzl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gwepsmmpc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gwjoawnyq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gqpbtnaar.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/glhfdjrug.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gvjuqvrmx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gjfiwumxi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gqjztrqti.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gvvvzffyx.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gelyhlhlj.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gcovxnjkk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gyivmwktx.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gzrutmgai.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtpcmsfpr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gvlifquaq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/glqvfrxkv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gcfldqsnm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/giafklkyi.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/giqctgsws.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gkhkmzxcy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gbfmtqrpb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gvtvfiiwx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gtuwroaad.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gtzforbph.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gvafpmxic.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gsizkixkd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdabzfjq.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gtmidfjug.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gufxwhvjq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gwtjfxghw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gayltnclr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gwmfprbam.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ggxpavcde.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gnmciuuzq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/glijhdhvl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gxtburybw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gyyvapxga.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyinxldvo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gjjumbeck.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gwffjzvlr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gniqufvlw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/guimzxrej.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/ggvxbjrnr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gqltgsbyi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gzgzqwnrq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdjwybhsi.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gsjdkkpqm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzjpigtbp.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gwxzzgfpb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gspzdcfev.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gsrufctzd.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/grlymsohi.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/ggyupljhq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/ggtyyiamo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gfsuwdqie.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gxlqlplof.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gqwktgjgx.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gvmcgznri.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gnrlmqdct.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gcecdgcvm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gbsxgreld.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gknbzsclf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/grrmbzygx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/goxmfsrgb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gmmjjlmjg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/genftvqlt.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/ggprelouv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gyzxlkerh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/giiwsdgqq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gfzjttirr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/grsfhfzlv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gasifdmrq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gyjlxddin.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gydstxgjm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gfkypwccb.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/govhgzdhk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/guvisfsrv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/goixntsef.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gipiqvqkw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gnknihzhs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gycpmjxam.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gjhflubxf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/ggfdwfqtn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gqnehqxjn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gulsdssjx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gezksheaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gbmesecyb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gitbtojoz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gkndrzgdt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gwhorjovj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gdgixuvzu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gzlfxatlv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbwglrxzb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gsnnyrpzp.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gdmhpeyvr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/ghglxxnyw.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/glumwmixc.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gzzdeqcei.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gstgrdfmk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/geuxiooik.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gwxquxzdu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/grsjjsifh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdmqmtklr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gajguwhzj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gsdwkoatc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gdjcgorup.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gsfrdfxoh.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gdkybuezf.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ginrgvvks.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/girkxiwdn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gwyavviqo.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gywhyixpi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gwvubwxic.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gzfobfsry.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gnhivewpa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpwutohwo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/glpakhxgb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gleplkrwr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gshtqxrgf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gudbqmywa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkxfufwwn.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gzuaksqgg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gebzsiamv.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gfaitoiwa.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/ghirxrmxo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/giasymwmc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmwbeczjh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gfimlqzyk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gbmrquzyb.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gkhoomtyh.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gwpkwoejq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gairbagtn.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gbecsdaxe.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gcpjmunwc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/grwdoiczq.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gbxerzscv.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gxezuhlkr.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbyhygeta.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcddjgtfh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/ghbajrqga.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdglzafbf.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gzdlkllsw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gzyuvsdhh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gxvdpyeoc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/glllxkmsn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvulhfpcy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gjueofgvs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gipelvcnh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gczaoduoi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/geykxschu.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/grorlkxwx.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gafzkccxx.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gfxsqhhrj.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gwsvfjvwz.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/ggflhmfvl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gubrxldop.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/ggmlmqory.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gqdcakuxy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/glwmosnls.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/goiduwwvy.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gnpwhcwoa.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/grnpfrzbc.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grhovfons.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gppqfrobw.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqgcehsyc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpbwzhbya.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gidnsdwjw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gahltzozk.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gmxzfusia.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gctczmwel.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gwqxdvgki.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gszkkxuhv.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ghgmixpbh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/giqfevpua.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gxwoqoezt.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gqzmqgial.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gqrvztvdr.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gkvcwujdd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gayntutbe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gdulgghye.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gxtirzmwr.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gblnchffv.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gprujubiz.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gphsndxvx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gkkjazlyq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gnuhbmcje.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gipkykzis.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gnafxfbax.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gfzfqvvqj.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gwzrxolje.sHtML


<!-- 参考信息 -->