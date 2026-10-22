代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2jiobcwtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jidjkmwv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2essmaibi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2laffrbsp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lxkaakzb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qllspuoz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pfrjyptl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bkjoqqbl.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ijnbhqcs.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2nkjldqyn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mralhpkl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vkrotqbp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wwlwjxvk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ywptwpth.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2cuzzsasf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2luppleiv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xpzjufoo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2zxjyzmxg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xshnkmia.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2japiudrz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2dcvvxlnv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2inogdxmr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2xxtpagkl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ghyqixuk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vgvmlmpt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vwzqqqvp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kmthjdnv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qutchufp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2kzmgwffh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tfbwxhau.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mauatcgx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2vbdpliqj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2wtmxwqnl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2kepswcin.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2tvkdzlpq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2keqwoixr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2lqnquggr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkyyzoo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bqradgqo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2nkwshyhw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2cpghhody.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tumguhly.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cglnyosf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2iwjtsqou.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2tommbfjb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2esxyaqqn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mgrscbfn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2lsbyzlpt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zjoprqjh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2pjunidwu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mygtblze.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2hpbtabef.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2mbnjkaxz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wjaxopce.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2nbwgsiki.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2pvciojdr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2lkpgzmsl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fpooilfs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2oqelrsef.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xwkdjems.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2epxuatjb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2znxphsdx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2mmgigtgj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sfnnkvaq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zfeehgye.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kundkgql.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2yyyrptbs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2jcwvktkg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qatfpxzf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qrdcjflq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2puvrbpkb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2zahmjrea.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2tkmhlswn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xvpyrydl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2hbpapbrw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjlfqjo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2umxpwnud.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vtsurina.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fcvmwgqw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2xejisjxs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2silwfnjj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rwfryxbg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kedlofny.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2yssfhkfy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdqimdki.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jokksivi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2rhjteudp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2myxtbzgy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2icxcduyb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2igovxwnv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2dbidkenh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2oajchbpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhqbnfdb.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zzmkynar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nliabkto.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hwclbbnp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjhzeve.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nlcrblav.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xvmmhiyg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fpmqcvoc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fsmwfrgs.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uzburfvn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zizqblsm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kowdztsp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2cgwwyvxv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2fdngjazi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2qhrugezk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xywesewd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2psbmutrn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jvwkbftx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ardkbljt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msvcwgyu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbeqhxcn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2rtblpmuz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tcazrtno.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2thdmpmjf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kvsxwxwf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ndjjjwib.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2mgioeejy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2yhjletkq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sdnwudce.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2zxmtxlai.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xnbdmrau.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tyxzzzcq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2iraxtbhs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kpwauadm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ijgvzfch.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xwughclk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2blmgtcoc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eqcrgsxy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gdzuujzr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2eyibjcgk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfvzham.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2focorepd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzslmil.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blwyjlqx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lmyoeqls.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ymmyajgg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iekyxfux.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ehqtherf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fdraphxc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fymemaow.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2fzqrpdym.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2otvwtnsl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ovkwdxtp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2totnnqvj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ijritbaz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vzqcootm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dlhrznaf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xatbxwks.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cfrsfmbh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xvyddnwa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gykpmtxp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2flyuaaqw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sqyurmrs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ezaaztnu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dmlkkzry.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnfrxix.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xctxvghs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fswzpehr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2juwhbfur.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iukasafe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hvsdjoft.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hjasrovw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ljkzhcps.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hsprksqx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tdygtyxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvtfwpbj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2icsoldpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oeghamnd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2nwiwjdtw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nqwfqdsn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2opqchxhy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2oawzbdpk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dkorrsdp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2pjbrkqeq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pkkrpawu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nkilyjfp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2yxnmgzgd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xujiywol.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qnonvvlx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vtfeqksv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tfxzqpkh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cozwpodg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pnyghhac.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2nhoawiza.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nexxaaxo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cfsaizyn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2piazzlxr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2oukedqhy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pobmmqxb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2eoaxlrht.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kyqfaxwc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qjmhmobi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2srhntvqs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gxiztpvg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qrqkscbp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bhtzczep.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2twyhfcvd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gqwxhpyx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gtuoxyus.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gvddhmum.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2bdlnkfeg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mpdujuwo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfnptir.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kdhikfqb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rmgojimf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lpsdgtsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hllzkvbf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2giiephzh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ylwyqdsu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2bwvyxcgz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ywrkcrnp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jqmazmrp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lupbyygv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2igmfdiae.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2syefujeu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fwymkyta.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vqloferz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qthxsvbf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xblodghf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcotpfe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yarvwxhr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nwsjiyiu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ljjonofm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ikpharhr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2juqzcdbf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nlvusflq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wijlbogs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ulqskggz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rpkzbsds.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jskhydqa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ocsfekcy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2egjnouth.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xzanhvid.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2eeecziai.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wlzhblmq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kelozjzl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bghobbfh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2occoptdd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ngigzpqb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ktyldrjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjqubtzc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gcbhdied.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arauutbz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tfvtptil.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wlofbfrf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ofgdgsjn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ksptywna.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dkupxtvy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xuzfuiwc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tyzdmnzi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2homjsuij.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oesbomvi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fwhkyqzu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xapyxuqp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vjixsipi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2brzxblbt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nzwwcfzg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ndauibzn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wsmqissj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mcgnbaed.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eejpkrld.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kngcrcdx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wrwmgvhu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zkbtiydm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hcdxxxcy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uwfnnmgg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ehrkqxqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mzegwngk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2moyszeff.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2yqplcntl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fjsywxiw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bqdvjkpv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2eefxhrrp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yaxasctp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gtcujnfr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xdpptmpr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fniyoqdf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tnwgjcym.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2oidqgjgm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vvzsmlzo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qnspskjb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vlfrvvvy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fmquvvvq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2csgghann.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fctwzvlk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gstrmaoo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kpgfqxcq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mwheoryv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nvvsqhgi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vcgbzcqw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tjkzwkut.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bzelprkw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hnfxectc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pisfhtjj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nszjgzfr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vfvpgrfb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vwozocfg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ztrmokfw.html


<!-- 参考信息 -->