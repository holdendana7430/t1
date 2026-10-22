代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ctfmqllw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2diwqrekx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2erfaqawk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jscxesqk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2takhjosg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dphoexiy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2lrwyzqtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpyceppc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2vxmrzmzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjpvloiy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2qotvjcnf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2gwevoxqq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wafnynnb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vcdzhpoy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nedaomql.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lysrotfn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2fosvdjnd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2iaehlhdk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mwviwwxt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zpytmlau.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dtzuqkme.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tzpuxpxm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ikwqxehm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2insdlvgb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2hkxaziqa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2wzomyuuo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2uqsmukbq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2fcnyvjvn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2psvldkdx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2dlzefibb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2botirxny.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2exnxblsf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2utypwysh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fhmrdvfc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zmanmjjb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mubuzfkw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2bubkloda.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2pfjekjhk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnahbhs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2psokiard.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2mturrmoj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lpsrrjcr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mmmchkms.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2osthrjms.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2zahbmfhq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2depxxtsg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2xipsflyc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ivngtwdf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dhcsvwbg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rpjjpwpy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tzgyqxgg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2aogcckwd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ozzbbqrs.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2occikvbd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2uabvyhku.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2dcueilhf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2uvacpysz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2toijyicf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2dtirgxbv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ncjypppe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gfjemvwh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2xqbfxjkw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2oxzzrozd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2utetnuiy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tnopmsst.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xgvsozne.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2sjyfcxtc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qcprxrjx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2azbyhlxo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2chdigifv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dmiecqqq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nwlgrguj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vltkpacu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2pxzpqxda.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2khbplomw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2jvvrcfss.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qncpuzmk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2wluqhcke.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2nqwuclhc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2somtwvfg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lppgrgln.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2uclruwzb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2kzorxkaq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkbnwvr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2guzhpbat.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vqiizqpx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mfqtcqbq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2asakkyrr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2suixxyyw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2adoemotd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qjpmlace.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2numvphxc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2rqyejhid.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2udcqnlii.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2atufzzft.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sfnphnag.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vjxplsdt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wbstgjhs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2trfcdgcm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2zjnhjajv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jognsvjv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2lrnujxko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qilouopb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pmhihnik.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fhoptwki.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tsuxjdaz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ivyoaxkl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2letjhrsj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fmcjcmvb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2wuhfrsae.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2bcqgbeja.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dozajowg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dsalngbv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hsazkrmp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ozidabpk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2liiyxnio.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djnnmchx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dwskqjzg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tsmwrpjl.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlioxela.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2woiejfud.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2zyypmkzw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2edsujptx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2okhdiclw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bictjlnp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmrnnyhn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jklskgmq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2akfptkji.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwhuihv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2rbpfcgfh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2acrrnplr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2wyzanffb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hbiuetmm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fnvgsxmf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dleolwxx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tvcjzrzq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2itfkgwyw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wzgcqzxi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ztyisdys.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2furadmza.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zozcceih.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wbspdhed.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhojdlvr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2anulmjbk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2exmbuynb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vlwrqfxv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yljumrnt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zpwoutch.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gjravsce.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ehpkpvqz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2serlgoxw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2inxdbytb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fchzbdxp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vqcwqcth.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2leiymusz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bfkakgse.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qxrldfzi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pvqfynxt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qiigtpig.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2rflnnjcv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hpgnsacb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ujfotmxf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zswoqnua.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2awhimpsn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2sxxajqvp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmiichg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xohztyol.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2adtdxjzg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dvxtuqua.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dtoilukt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lfwljhzd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2exukyhhs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mmkptkhn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2davkbbfz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tbcqcygf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xoljxoau.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ztgnagza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqbuvtjj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tyqebwgk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2apduvsdc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jfxijccp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2apkydqya.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cuxzzsjs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rhproven.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2scvrlklf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ettkwqtf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2bbcfbjlf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mglrimyo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2guiqhcek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lnuxsizo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2udfywbax.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hjyffrjv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2omgizvus.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fmnkbwon.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2glmfggvp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cchoqffu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nssgrrei.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2noasjfyk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2efyleswn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yvshphto.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qhdwghvj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2pqkrcmoc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bxxtfeuz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fgtoxscj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fuvxgsau.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rytlbezs.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2edpyfude.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hltyqskg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2edtyqlwr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dysfrwxn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jdhohmat.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hjjbqbcy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ucowipfi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nacijcby.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hwshytee.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2soumvjdv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wiysuhtg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ozgnejza.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wthrhqbo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fzwgoeld.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pahhgebx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wzspzkzs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xoehzthy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wlkymnps.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kfjmhron.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zqscgiiq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kvmkoulg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ccqzbnlc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zovztwgp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxhjded.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2njtuhwki.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lqwmwwwd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nnatbnlb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tfnbrniu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2otheqfuq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ezrfjbxr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bueqclic.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2irujslij.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tawtdawe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2egloodoj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pwlqupck.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wyaqwacp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2csqtklmo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cucfpojf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rdxmhpbx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eblypskn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2yeqkfvni.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2sfjwghvk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gnwbjyvf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vetahjgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxknfhhq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lpmncwmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdnyzbwz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfyolomk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qzohejcy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2naatxbyj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sypzmoeh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhyglqqg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rzeyfxyb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wqhpuead.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jbcqgomu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eqvcotmg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdzezpvg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cwvdfrvj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mdblnkue.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bicskmok.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pqjgdhla.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2plillhhy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bltiwgwm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sxuxsjsz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hxkdlnsf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hcucmocg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hapsxlro.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dqjfpfkr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ythxdgfx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xtxtxehe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nmdinvvn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gwhdvjnm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wodxuvsr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tyxwuqgx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eojgzimy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mfnmtmbg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rncwhejs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ehzdiljk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pcllmxrg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kngohudu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wxclybss.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rrvdxaui.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sdfzfbyf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lnyozdtj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywbzqhyw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hrpianzl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ynodhvvk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uxymkhus.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntncejgc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2msercjpg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ortlhiuy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qnljvdhu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mkgapzqx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pgebxmsu.html


<!-- 参考信息 -->