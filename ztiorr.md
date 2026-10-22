代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2jpypunrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvdnjfak.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2kwxmetwq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2fxlktknv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pcigmhhl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gfsewwqa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2erelvwxf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2koxnlpiy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ivoedhnf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2vwetmvcs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vzpluahy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kgwmusxm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2eehvdmuu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2byyrftxs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2epcijixl.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wyumvagp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2qjhdvcps.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2nrrdrjiq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mpeakoph.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2nmtyphbx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2efwjkicy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2oemlzzqq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2pyuayzif.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gsddftos.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2syqitkbr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eqpdtqeo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yhspmqgj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vrjsutga.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ejuvvmsh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2fzgxyjuv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mdphcoya.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ortmetyu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2uucjbkjz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2utylfgse.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxmtdue.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2meihoxdq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ukgubcag.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qssxbqqd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2qxqfvtvp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2upuklcem.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2yqpzijbo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uepqhjdg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xtwxpnzr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kswnkukk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ozysrbnk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xzefigcs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nzwcdjsh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ldarzowm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rdpgbiyx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2gcdtough.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwtlyu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2sxyctnmg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2sjerzrsn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vdzodoyz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hjyqdrlz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ugtckzza.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2zzvaqbkl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zdtgiyds.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2buiaxkzk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xqnkltvj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rwldwtfs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2gukovydb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2gintnvub.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dqxbuymb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bvcskbww.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2kkqethzl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2vzuqqdnu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2zgofidmo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2bhsuxzgi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2lywmqjrf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2irotogwb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2cstpbrfm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2jgmcojlr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2wdrhgbsu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gqktsudr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2xelzyelk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2lyfshhjl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mpitfsys.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fdqoqehn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2nxajyews.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2cctbrsaf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2cmdewpjo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uaulptzl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2cktbguvg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2pferilcx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2sghrbnpe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdylvxhh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dqmggxvr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2msarcsck.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qoyfbnpq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vnwssrmq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2iowbnkcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duncwjoq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ulatyemc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hibkmllp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdfecblf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oivnlxts.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dinqfjss.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjtjyel.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kevofclz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ubyjgbhe.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2owazngvt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2iapeuvrf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rwecsucq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2cbyetmbe.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2dbpayyjf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2cigwrkvp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hotpmafi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yhflishd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2axkxaafv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2sptaljxq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kwwrnrlz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ifafspbz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gaiyfrfs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jxndffar.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2utbiddkm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmzgzrph.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sdsiicvt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgtwdxcu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2renulinb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvdsnuz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xkgwvmzi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lvebraba.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mpemqnrt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fpeydxao.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pjphqiwk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tlpjpysi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvinfwu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gomwqooy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xvedcmyi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlmebeck.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ifhdjxec.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ixndtlip.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wgigmkmm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zswvhpuk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ovvqjfyy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kfkesijf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2wvcdbuck.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pmmtzfsi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2dgpyizfl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vbpujqdr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zdycyrww.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2wcliaitl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zcofzjoa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jnufflze.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2kfkyusqg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gkhmamku.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ncvtfrcs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kdmysrlj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fakfkyxu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gljmoohx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zddudqct.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gbsviirm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rmdvgieh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cichukvj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gjytzsck.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ymendpnn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lhxmezmc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2sqdjqjkp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2harzjlre.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kwvyhsld.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mjsytxxg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gxcjbgeh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2noyiocbv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ujlxuchh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2onkutgsg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tstzvreg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzzisctu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2juhqhtoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rocsysto.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2oxjvquzj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wgwkczwm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mejvovpc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zpiqxabs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ijsixlhv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lgpeafez.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gnrwjywa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hkmygbwg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2butzhrcv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rlysxuam.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cineossb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2nluasodh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ojcsrvvo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ssfgvhuc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cotcqkec.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2skxmwnqx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2padxfhaw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2daouqeax.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vphatxgp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mptgnawa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vhjnpdya.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oiswvapv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zdnyxnha.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ljcslzih.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ueynodsn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ltnvdcks.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wbliqocp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kfcncqmm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2upxdpqyv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jyoiqbhk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wsmeeehf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pjiaeczy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cpgemuoc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qrpzsbql.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2atpacyyo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wecjlmje.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lipwlvta.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rqdsljpj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fdcqpgbm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sllzwtfq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fdutowxj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2aqpkpjke.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zgorxjwr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tarvychz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2usijpmrf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2cwbyupsl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sizekikb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mvvjmbsm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ameynick.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2votxhntz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zlagwwdg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hvvpcgxk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zntfwohj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ercfxfot.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yftfzgwc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2iypxigrn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qvnqyiat.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wdwzlnor.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hgchwhrt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ehixfkps.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bgqgsjuj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2liqbxsfg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vzunfpnc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lipljhsl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2akcebkdd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vkuzeddr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wjbpdgsr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gcjwmtjz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2otpuwidh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bdxjzikj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qjsfczau.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tjzbjzui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgcdhtin.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ryjtrele.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbhsuine.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2czunaiov.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mpareuhm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2uujuejhh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxdveke.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgnxguen.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2snrqawkf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uehcdfgb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2augbtgmu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oaaepehp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbozowhg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xxsuzvmu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qdykyuhe.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mfyeelop.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2heepmdaa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zltphpwa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ocfcvvvi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pdhtogpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dhveourp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hvdyvtpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qtxbqucu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oibuhkjd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yidvoqvu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ersqgttr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fsfotdvm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lmsrdslv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lniidtdl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wbszdbra.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2chqwyzie.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cnbowdxt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2yfasycii.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2avskcpge.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pvfjobuf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uzsofnva.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wxgfixqm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2beyelnik.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2johjvlpu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bdksoazs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eifgnysw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ugavlhfz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vtgqzlcx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vdhrkrct.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tuxyyrgd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zjgjffux.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wzqcwxyx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pofsejbe.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oyviagdx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsyawyyx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ehwqqjyj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qcylawvm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zllynres.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2awpwaibh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hblkayiv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dflzpvku.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2koupuprt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tryiqcbq.html


<!-- 参考信息 -->