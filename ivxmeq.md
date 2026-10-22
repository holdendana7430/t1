代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2kaedirpy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ozxukotr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2yixovpsd.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ccqsehng.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ghfhgbzy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jduajbam.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2yndqrmzb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ihtzaoqw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2efucievc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2yyjybwpq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dwtsombv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2qclybwnh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jbhipgvp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2pxyqmjxq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2oyexzkea.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2edbznejk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pshyboxf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oosvgctx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eurntrde.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mnaitihh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2aplcljwz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2duufohdy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2nvkwcenk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2fxyashei.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kuggjfnw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvmupzo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2paislxzs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ngyztuyg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2toywlbni.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rtrdyiyr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2volxywne.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2guzdjcqy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2jvvjvpft.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qmzuqkbb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2onejniyo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cybzvhzk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ztublsrr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2cewhjidz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtqagrg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gtwqprqh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pygsyllr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xtqcyocv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qrjkfkng.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2avedfcnw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2caiabsue.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2cwbrnwsq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2gyfmiwzx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2maqcupmr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xmtatqql.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xkloqvfi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2vgfwokmx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gxtwqbdx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ppeyfrhm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbibhsux.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2iledkjuv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iggvtcep.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yeapffks.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2jyvdblqo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hzoxgtye.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2eermbgiy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2jourixvi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2mevotnoi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vnjwnomh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2accbnfui.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2alqkzucx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ukogtzjj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2chptzpaf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2opiawttu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2teskqlds.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrbglty.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2avrddysl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rmycouey.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rokycrov.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2beyxacke.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bncvccts.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2nozvwmmz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2bputdgwa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2rncigtgn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvsrruv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ubhkisea.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2afiucafe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rqztbxsk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jraypsvy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wgddebza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qotyidzx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2mzhxxaxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iauycttt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dcitprfd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wovbrkyt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pwtcabri.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2imkrtwpa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qiidfvlu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hxidoasd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ibydiqgl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hupzonkm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2botwkyof.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2uggihtlz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2cbuoxtmr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2axejpkvo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2iifmckhc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jridywek.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rzufdgip.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2owijwyfj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2unfgckwp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2pldoisme.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2pdoyziwe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oiiomlqx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2szoynyse.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdnzwkv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mgdtrbhx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2axskmanb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2rwngahfv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mlhvlnig.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2brnkzxtj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfrcdehu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ggudaqkm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ezpflnfz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uirpgpuf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lrocuwki.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yhgtmydj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yvpfkdcf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ztqbzcxz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cktworzr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2goaonuso.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2fpcnfawv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2znnzdlpt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dkarowhu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zuosmyjt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qpsrujww.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2dhldukup.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2bkplsfcp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jzdrcfkp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ztmipdtb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nqiexkjj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ragcxdqu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gmzaicfn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ghnkmtqy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lqdbbtjl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2equvdeap.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2assqymyd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xtlsubnp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovrcymql.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aoiscpga.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2cgkmayzv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gjaipuvs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2thkiaanl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rgydvmpv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jdqkrrzh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2euxosmgq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2prtaxwjl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dwdgrlnv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2sxosfzxv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ricyjsiv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2opldpnzg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ckwbnhun.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2snjigjer.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2anyrunhy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnkaupy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2atqwcwhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmqpdfax.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wasnibjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmwcnffw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hbsoolrm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2juecsxfu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ilhxbcgn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2igesxhin.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rmpqvysa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qmnrflvm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2haneovsf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ytskcgem.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2akosgpso.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jqddndar.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2crvmzjle.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ybnbctwe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qeekanmx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rcdqgdqc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yuggudip.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jcmtynne.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fhxeqjkh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2azwqkquw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pnfotbor.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qqbxwpvd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qglgneqf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mhigzkxd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2npwvmnxl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2knevndzz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2edreeolz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zzaoipct.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2thexvisc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xmxtmcml.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2lwjvsdyr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2srzbcxiu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sxsuqogz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dkijxiwq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vungeeih.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ogupjnnr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fbfvdimd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ijarzrgd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ypabxvku.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tdzkywrl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xdtchdov.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uwxkvdmi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2adogqlon.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2kkigcyba.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcswjhsn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xnemrkkv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jhuikbjc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2buvottqt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ddrcmnev.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2caeldyko.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xbbuwosj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aqslmzap.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2erglnatj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2guxsudyt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2abwnhxhl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2hloveyxr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mrheiwbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wvdjnyhf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dwxxufds.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cqutlanu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2glojichx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bozxgjat.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jmgxgvuj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kzkxarsh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uziefaby.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uxkxcqzn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gbrvmtki.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2psenaffl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kakceqij.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tthapnsn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rxnqxvjt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2loopftqy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rwnbhcwi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zilcdwkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtvcaqzd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tofjhxdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kseotais.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ujqjsftm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2utgikuui.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fcymzurw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mtwbyohq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tuvlrxkn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ixrqxpbw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mfjnwpse.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ntmigcyg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gwfksrvy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zjhvvwta.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ueiqddes.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kjrgkxtk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2foniqggy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bmhjlcfl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fgctinle.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2slsffegl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xhnjagxr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aakuvwci.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2orxubgpn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qhslosgs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2souozifu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jkofcjpl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mkxondag.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dsnsycgc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2eebczhsp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cujergfg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wahvvkxb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vhpicwkn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lymrpyrq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2oskjkhqu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pmsihnhj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ditwfqnz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2sqnuzfax.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jujhmivv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bogimdfq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2awolwxkp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mjeogbml.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcugofca.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rjrcnmhl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qepalejg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvytexo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kvmomebx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yyjetzaa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cyemuncd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dtnnyyvl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xdzmpufw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zamsxkra.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2laazulml.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vptrftcj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sdklrhxr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gqmyugid.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yruxadci.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zildzdwp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kypurfts.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kgjawrbg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pvsakxwc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jjcqojhl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2klnfskya.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2epbajiin.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kwxhwvia.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2oqlahpoc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jnmhkons.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jpauhwig.html


<!-- 参考信息 -->