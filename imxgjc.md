代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cixnooox.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wojsecrp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vsslrtqi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ymlhtrpm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2igsdxemj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2dsxkuqlo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2aavsmqng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryhxcjof.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2mpzupcbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2catkcsos.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hstayami.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wxchzddd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xmbrvfyc.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vwggrxng.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2fclnjgek.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qiayaiwv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2hufjqyfp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2fmlsdsqp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mydojlnw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sspwfzyo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mgfycgpt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2astcopak.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2obwlffih.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2snirohnm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2kyhbxaav.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xzkirart.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rtdjnxap.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2rwhoqmjh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2aefggecj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2zuccrxns.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2qaotcgac.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tbvbrsev.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2polipdgn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nxznicul.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qxvhwzlb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uzaotdks.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ccbxmrxw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2hlsrpfbl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2msgmmaml.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2zcsfsspf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxmjvmz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2eoxnlaoc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2gosrdzuf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2dvuuktmz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rnwwpymx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hovoslie.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2azivygge.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ugrbcpal.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2hlvcbcah.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mwebabgk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2xnoimxaf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eipytdum.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cwivpdoc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tuzyknov.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tlrxqyum.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2mnvknsut.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ukfwngjj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ulmruxwf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2fyntydva.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2fhmhouqn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wglhiill.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2fqhzypgx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2isufscpk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dhzwxtyr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bcxhsxwy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kgysdufc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2lauanbqw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2asnnymal.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2htbigjso.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkjfvhau.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmmufyuq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2apcabxpz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wiwnvqoi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ldundrns.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2evrtgdhl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tkxuyoav.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2llznohwa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2srqdeypq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2yhhcecnb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2qdlklmcz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ccyzutck.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ingylumz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2zxmhmisi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wxlyksro.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2kadqsxvm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lachvkjm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2phpcpnya.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ksyotjct.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kdphhwno.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ziccmzrb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2njlwiqck.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2teynanhw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpylbmop.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2kizxmoql.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2duermjxi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jkvqwggz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2aasgelik.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jgpymjxt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nefzpocm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2cpevvqmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kemjnztn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ewcxeiqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myouckll.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2likwqzup.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wnnizlvt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sxoswgfh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ymptqies.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cpfnuajk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2duurazfb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2kitzowcl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2eybvdury.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2lurjvmed.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2szsbokja.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfnwbce.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pgxploca.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhpvpvou.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jfjsmhpl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ublwnkjo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zvgcwrah.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oomghfse.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2euamkfkp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2hrawdaln.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ykswnlsj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2drzywcsb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ujdicpxv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ejgmjyrn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2lzswchok.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zsqisprt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2tbibnqeq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2epsxpvdq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2erqjzlfo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xwowwqty.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2jphmydkh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mprhvjdn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uiocmgzl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ribwgbgp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qwdyvmoi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezlxttie.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rkasdbfs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2hyknntak.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2cnytbbtq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mhjvklak.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ldqqmxux.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nkmmlwlh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2zmpketej.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xxkpgezj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mohjwwkd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kxnsagix.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nytqkgqw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yyzjxoes.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jlzmcxqu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kequepzd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqbwjz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qutcflra.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rwjpqaox.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gvfpixmu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fyqvohdb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ijebzqdu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uhcmvufq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2rpwqpyht.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gjvbypql.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iuyatotw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uirlipkl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2otzflxhx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mfswqoaw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2euewzcor.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jivrokuk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmnkwbe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kevkyfgm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ucnhbtrd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2frgtqbyj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pmjffmxd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2atfblwmd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bcporeoq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2godlpjqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpgtwdrv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2uuajiheb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tonyacpr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2uwrlugna.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lfffcdku.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xzemjqle.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ugjzfeiw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dzfyvbwe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2cjpwuhzb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hgpirkrj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2uwawhmxv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uxnbuifu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2muvivbag.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2twynwxwd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hgeegsiv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vndhinzp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xwdynyvc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dppbpmeh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ryrhhrfu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2duhbhxtd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ezdscsel.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2hghyviez.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2aiczraia.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2obvqtueh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nsshldvi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2emxtgifn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2svwllziw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ddiqefjy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2exwpzznm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2limerxzq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2suarrult.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xtwffubv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ylbmexau.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2etaugect.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nskfqgak.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2kjnpxxhp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kgaoygpu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrobyql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2htjgjupz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2skiynufx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2oxrttqbk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lctvxysj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rdrzwbyz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wqqgfthg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2dmwupjka.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wyrscweq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mdbqufin.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vcrjsvba.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2cufitbtp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2isrtzmcg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nqsbdend.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xeqhoode.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jstjbfsy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xjgmccpb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2oospxtie.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2twkxbhgm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2hitqkiiw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2khwtvtmv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2apeacnwr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dbbhukwd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tcojoqjf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gzvrvqut.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2uyidxavz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2otjbloen.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2feecamol.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2umnpifnp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fnsdvjdj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2orqdrpdd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wufqjohj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ekrwvjbu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ooeiaoeq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bdifcqrd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bqecdwdc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2olxqsfpx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fxozwrkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvynzsvw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wponaazx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkxxyagz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wjmlvzcy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iwxoaevp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fzcimreg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ddjtldyi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtvuaqsj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rnreozvi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2pxejywka.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dwxugyfm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bwcnysrm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fclnwimp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2byttbmcy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2txhhujwk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rxfhslix.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gashmofi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pvqtflbu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2belymrjp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wsiujrsd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2smbtgzom.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gfslhumz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2twzvfdcs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ftdzedcx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xjyvofec.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2juuqexyn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xbehjbxo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2sfcefjgj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vjmzyycl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2upmlgqgt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2thijsbmq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dtzutgzx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2burhzyer.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pskoutxc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tutiadqd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hdazmsfu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zluhmwvx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2msyuymzw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wowntwba.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tqrywwgg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yubmowxy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2llbzqgcr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnlgawmb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghdxqnhk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wocavcsi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tdudeobb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhyzbknh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pogqpuun.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fhvflpem.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dxzgebcu.html


<!-- 参考信息 -->