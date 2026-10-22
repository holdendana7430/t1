代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aiyibqll.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gnhipfvu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxnqkdb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lhqpjcai.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2dsodcxlp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2xrfcnilc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zwlnvztn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eujbjekj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2hobveqaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2marowgfc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2kzadqgqu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2myzmkrfo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2taahzktz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ltxgytwh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ptamlyar.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fmxjdlkv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2dcleylki.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2txjciwve.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2riqbwfac.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nazxigvj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pxnqxurt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2cuojbtsz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yrbcxitr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2lymbspdt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2evlkdris.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2bskojdze.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tsdtofxk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2lgoqdbcx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ekeokamh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ridimrgr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2wwocqmbj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dshuingi.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vbohetnm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rrmnigrd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2chgaltxl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dclrwcya.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2fkzefpoh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2uhoujpkt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2bwkvtuuf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2aamxaeri.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cpplhaqd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2eumpolse.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2wfflgeon.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2bulfjwzg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2hfdhzrdz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2elhnpvdq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2pjhxkwcw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2jnocfcug.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2zmeozhoo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2azqaotjq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2htmosyjv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wfajlqie.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hodcfqew.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2pibdsuhh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cuzkpdbw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vuibnvhm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2kwxixswq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2vsqznyfo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2odwptuqv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jjsstcur.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2aopijtfr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2cytxnfpj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2nghaxrfl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ilfvnvqt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2haukqxzu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2drwenskj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jluvlbtc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xkhmhivf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xkramxmt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2uqouuxib.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qibuznnx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ujdrneso.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vdxcaiuo.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2fnppawoa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jzzezrbv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2uecbfuzh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2jtsiccsk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2kslxyyst.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2bxaydxjt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2lhoqxhpn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2udbzsljj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2yihcqvak.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rimxgftn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbqducp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2dixmweux.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xihrwzzv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hadahjex.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2nkogebhc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2zvofnkib.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2kbxebptg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2artlwlnb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2cexxpnqh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2vmtslrzg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2yjehohyv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2roujjahb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jhluglkf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2wzicpwpu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rypanuff.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2girpnrgh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nbwiswfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvnpglda.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ttrmycxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxpmxkni.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgqguylb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mjegysif.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2raltjcqo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wyicskms.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhixpeh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2huuyonym.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2vsqipksw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ysupnhgt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ygslgnrw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2tnxpzioc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpsvyojp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzokuw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ameyqbsr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrojaqas.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ppuneezj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ealgnzon.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxlmpkrk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ueqthmht.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bbtndpsc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuriqlq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lfufrita.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qillxpdr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kydrftkl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2vadofksz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2crlakdlg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xsetdnai.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2wedhlzsu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2tfsqggic.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2frgbmlqx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hdinzmlk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gnwcnvrh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmxqkhcb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vmibbzkn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hhtvsrkj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwimgwag.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qzsngtvg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2vdskufnl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jvivalhj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2kflbhqzi.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zpjnhluj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tuegonvf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fzdqszok.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pkeztaqd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2nqnhcjpw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fdwmnjbv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qvrubxtz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tjboimyy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ealpfgyn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vagxzcsa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2sqrpjbbl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2owlmtgna.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bejianjk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ndsuivdc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ezxbvevh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2wffvormd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ilnjvrsb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hlbljejl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xpbfatez.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2okcryfgy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmvlwlc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2dssljghs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2pcqopovw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hhdvjree.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2aokxrobc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2painfqyz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2bwalhvse.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lmnrqyei.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2izwssusr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2gxncfyyd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dkxjttqm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ymqjgpdb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lmmszrap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsdfwlzv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ryrxmnfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipknzhfu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kidqoshh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2zwmvysvl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rtazgdlv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bfipczha.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cvjgolwh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lmuawgfq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2jzstvdjl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wqunxghr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xpjmpehe.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zshlehrt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2oxuuwgfa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2nfmixujh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2irbwadbq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2htacczyt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bexpywry.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vwosfblg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2eguifowf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2grotupiz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yjtuzvrv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2funufhiu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hiiynqjz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xppkqykf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cukexssi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jrohlhgp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2aqktamlj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hfrzoejw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kbciynis.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gttrvyko.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdzxmcv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ywcohbge.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nqjzqvpj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bxaxreqa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2efcaopkk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2knnobtqd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vxtmqhrz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wccrexjs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vydfwxow.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wvgyrbpj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2resxeade.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rdegqaex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2efjumvrf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jdodybhx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2uqcfdbxq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jriimeqj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzvtoofv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wtujeuhh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mdwzpwdk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mnydgfpp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zqkaqzvm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ykggjqpw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gfataxga.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wechwcun.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hxgnaxjp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oinqhvlz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jfhmzntj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fpswnoyy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vqtfjmez.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nflzkbqk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sxtqzbaq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fxxoebir.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bkoqabzf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xqmydzxg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ewqmepfc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2usempupu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xaqhtsas.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2asgmgtrv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xvgjjvnv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nnjylgoj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qkvqrnuv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yvskmkvr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ygmkudnl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gvhfjjgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aytfickm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2snjcoztk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpstlosi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jupikoya.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ixyqdtpl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dmknsujg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qeemumya.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lqweawyv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pqmtcfny.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hmchjmxy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mmcpovqc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rzxvhazq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jafriuhy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wmggkhlf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rdpvmypz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qthkoyae.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bgoayxou.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xecriniv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fulhxamw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lcsknzbv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jqmlkfrt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ugqkkirt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2paeviclt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yesllbuq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ucalrdfx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fkhrhisv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tqketiqk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wrnupfhs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gmpatnow.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aefkjspz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2foteknif.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ahmbdqdy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fhasnkei.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nrzecfrf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2btpdhyke.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nyqcqcsp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fqgzqjxw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uwikjgyn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ipaqsfza.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nqvahzrq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vykjibrk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xtpjowwx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vdflejdv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bihvewfa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yuzatovu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixmjccyu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hnmlhqif.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2utxcfbdi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hniakvzr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgxkjqnk.html


<!-- 参考信息 -->