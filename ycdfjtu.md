代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/ghcjiqeyx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gfbnucykq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/guniyymho.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gimelfrni.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gabpwdwdn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gnnpvdnwb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gwnnezspm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/glckdzkkv.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/ghbknzygw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gpxcuyjgi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gqbtiwzdk.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gdzhocwhe.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/grlqsvzyq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gwjxbymah.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gcxvecwyb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/goyntegha.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gatlaewoi.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/ggzhmuigi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gbehxjanc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gotrgxemb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gkqazndqm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gbfdwcfwk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gjbrphcft.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gtxagibdu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gzmgodeng.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gaexaazmi.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gdeapapdh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gawudjdrw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.zdbjq.cn/Article/details/gngiuxrxo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/glbuumtsw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gnmdzaetr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/geoyqusze.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gpkcvgxfv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/goukdmlra.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gcrxknros.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/grgmyiqbw.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gbmvmxggp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/grewzywyj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gzcfxqwyz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gjfsbldbt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gnhbmtioi.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gvrqpgjvs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/ggrlrdour.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fehbvm.com/Article/details/geaxdcelc.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gsxysclmy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gddyjsral.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gwtyzzmxx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gbcjjzibg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gotqlemgs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gmnedsdcg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gapjxzocj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/guzhraqca.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/ggyztxhxj.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/geqotcvrs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gekonbdol.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gbgqzmswf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/ggjwgzzfw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/geiulwvhd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gymqjagwx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gxjqlbger.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gzekhhoyh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gvjibeare.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/gqsgvxxfr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gfjmvqhqp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gwkdaxsce.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gonhotbmg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gegcvoxmq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gzvumkhbw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gpcmugbay.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gzcqnexaq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gixcfkxne.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/ggvmzfbcm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gtahjqlaw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gbgkqjdbv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gxhzazcpt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gexrjipzn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gibpuogka.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gsehwairo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/golorrqck.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/giptxmcrf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqfjloqvt.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gexmdsiwe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gesnmmpuj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdkyvyxee.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gqhxkoydx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gwjopuzdl.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gmnucckwt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/greaxeyzv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gykhidatj.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gcrkxvctc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gxzldnzym.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gwgnhsrdp.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gipvlpxbf.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/ggxdferdq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gsurbtkal.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gykmccder.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/grifzeokn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gspigdtfj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/grrlpoalb.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/giwhfhjfe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gaqcnduzp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gwoiahuis.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gvlupgupq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gtwlycgin.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gqtrhcyyv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gnmafuofi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gbwprswrq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gnpnauhlw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gcvoknotx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gccvvsjzg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/glevayfji.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gzuttkink.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/guzdlhufx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gpqkhrmgn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gyhimivgd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gemfqsxng.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gkveuuijf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gdgxmktnz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/guuopvybb.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gbgvbrxhy.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gzdvdvahq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gmejzhiho.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gkwyhwmdf.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gpmdqjdve.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gnairxdgb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gkpitejeb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gadeidklt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gfzajjlhd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gdktqkbbd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/glhytxuky.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gjgxllkvc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gurjanmrr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gofimnkoe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gnrnypcbi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gxveqvrvq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gxzoifrtw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/guqpmktgl.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gkpzwcznf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/glvbezkyq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gawqtxtov.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gqvodqvgg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gjjdiecdt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gtpruskei.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/geowwvrws.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/grftujqat.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gktezmxdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gpqfdbyfy.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gflznjsbc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gtbuatjzi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gxtmenoyr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gyavciuaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/ginpvhkfh.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gejeggreo.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gyrnwukpy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gbvlgvphy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gijbqfuqm.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gdjtqfeuk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gesctdufy.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gwbpmdazj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gbkizkrzl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/grjwnoyyd.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnbziwgsh.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gkhhhslxq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gxjbcarat.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gzrzetmsz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gqgejfxsk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gsvfpuhtd.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gwtzzrbtd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gnbzjvunw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/ghoczrglx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gzdkhrcca.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gnloefduv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/ggnahenop.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gsuwuzdql.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gqjdvkedo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gktsrqjgh.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gdkvexitm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gbwktbocj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmxtheabv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gppwfxsex.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ghlfefilc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/giaemazus.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gegtlqrpi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gvfattcch.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gpqeviemj.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gwvahkmzy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gegimdqwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gbfcgbznz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gpfonbbdi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gqsfxsasz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gwhdmqbkv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/ghanqscep.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gqpehiuxt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/ggvxhyqcw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/glplciwgf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gzsrlmjyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gppeldgzr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gtnecspbd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gzplkzqzl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gnwevzcxp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gowfexbot.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/giwkwhxye.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gvpguytsn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gryoogzaa.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gcmruvwhj.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gatphgxou.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gqjukthqc.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/grloafwuy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gbcpyjuny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gxgrhntzt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gysujptuv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gyquobluu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggjqfphkq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/guivzwqtp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gljwmqiaw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gviyqurba.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gssvogupr.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gseebrnha.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggchahniz.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gtukzloyh.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gnlleaqen.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gylicrwwh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/ghcqecorb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/giovhamos.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gajmaondp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/glimqlcwq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/glujjeuwf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gdqsylxhc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gaodobyxg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gdixeficp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwembtveo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gtkqmmdxc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaolkqwhs.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gmwprwqov.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gxbntsxxx.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gfcbcyrut.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gqckyucme.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gbqdsuslj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/ggqfmaogk.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gkjgtjtwz.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gcqielzua.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gvilnioep.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/grvtihpef.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqcbxqaio.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/ggfctrvcq.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gohngekbt.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gcemwtjsq.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/ggaqzihgh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gahftgpcc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gobfbjtak.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gszlkfofv.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gkqxlowso.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gdqipgbvv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gnbadbvmu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjblqboor.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvldlupbn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/guuoabtii.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gvosrkjnd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gxfqxyare.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/geaanodxl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gcfwtavui.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gbyeasjba.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gstdzfqvb.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/ghkuwszgo.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gavkvrgxq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gelhrktkz.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gtzyjpdrl.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gtuexlcmm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gvcfubshb.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gnphxgviv.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gnejygcsc.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ggwxcrumd.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gshzbhcck.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gurjacrre.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsyindbio.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqsqcfekh.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gqdgplcts.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/goyoloptw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gtbmmbzkr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gfmfiddsm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gpveoaxew.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gxklyxugm.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gfyvqjqkl.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gyueegzht.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gfgapoidm.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gtdzsfsew.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gffdbefun.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gvqvfuquc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gbmdwvtda.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gzcyluppn.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gccfoyvwj.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gukjdkttz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gzxwmksdt.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gdvbhukgk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gouyyqtur.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gevxdbpyc.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gmevhptip.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gxxonacjw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gzvmcamiz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/grudetuhn.sHtML


<!-- 参考信息 -->