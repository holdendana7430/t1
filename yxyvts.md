代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ifshqrrv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mdrrmxkn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3kdrumclh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3svhresco.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gjgjllmt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3geempkcw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3pifietwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmxvuttd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3pgyhtfri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqwcntfv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3nvvbntqk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyfsrjy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3obadjlot.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vrkhahbh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rhadrlfh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ufpuivzp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3regloyuq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3wzimprvt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3uiklzgbn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zfvbibhi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wclhhnad.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3drerddje.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hhttgagu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3kkyzrsig.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xovijltt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cmqipubd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rcublrgi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3rasnevrm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3eiwwhipi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wmdiepjr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3agxeissd.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3baaclrrl.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aybgvjov.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fnrmojad.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3memqragq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3habqtnho.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vgttgdlz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3nkywxlga.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nbdxltbh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3oqpaaxhc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wqzsnbmq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3aaxzmgdd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3pfeyruck.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3wxyddzii.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3bvtssros.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3sjqhxxka.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3gpifvxtg.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3blpdfhzp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3nipngjqs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gduvxyfe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxvybtn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bzsojxih.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wrsbriic.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3kyralzzk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pnknzjfy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3byzyliqr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cbliqhlv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3bsaiadyl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ymhtogoa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ekydehwq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3hxhelbuz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3flontgeb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3lhwuhwvt.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3plpfsbvh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3qnydqzfr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nazlcskf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3tgojnsse.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3upujkqan.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3scwwtqyw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3isvzxrlm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3jloiobmh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xbdijnvd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zbggenvr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3lejpdhsq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3zknwfmyw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3uzneubbs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3huaoacsv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3kljnzhxu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3eklovrhc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3pfboozim.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3fmfhfgki.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ogkzzqzh.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jytfenbu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3efikdoev.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3imyelqjg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fiujbtro.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vfntlanj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrcowlf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3yvjkkfby.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bhhygezg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3wobrjsdj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3fjzpwdrs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3kkdwopid.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3cqztjqcm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3dklroqdc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xdehgifz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqcozsp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3wswemkyp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xvycybuu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyhhkut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbehfies.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vhauzicy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcxmcvph.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uetxhoky.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3huhgvpke.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rxfomvpo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjwvskrf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ttylmbre.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3lehwijio.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqpsphuk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qmefiigq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fibdwhlo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qbotzkjn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3kzcuymse.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3fzbbmpvu.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggkyhmqr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lfuqyain.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vmghqnwg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ubezhgcz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gowtwbfh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ijyvwnso.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rqifowav.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcmbgar.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yverqezv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bmpihsvz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shegsjud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkxjqri.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3leeezfza.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hrcamdzv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xihqhxay.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyapdfwt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3oozmhijq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3slyyodqo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dzupxvhw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vowgolsi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oegwunpg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ffzeuivr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3akiycztd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vphwhywo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3peehxqtg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3pspzlbzy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vvivxevx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mtvzlddz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wsrrzmew.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ryceeipz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3upzhzcpc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3snykwcnc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3xjvlfjsz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3cmxdugsd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uchzmwcq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ieeqxyvu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3flnvmovx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yenlwiys.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tmgkugim.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3raylogst.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gxwfgoig.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iztnoqat.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jtfwecmj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sjhxksyq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pvtylvpy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ykrulyhp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yhmbgvic.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nsribzmp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nygvhdsy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ksdrdjfs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qlpjjney.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cxolfpml.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lowidvac.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3panogotz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xsgsbjva.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3szflmcef.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3wxbpnkix.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xwdoaiqe.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqnmnvvo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qtiraklv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nymcpyey.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3uutjofza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heejpunf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3avwfwzxu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3owqywrfu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3idktkgrr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cfcdlupr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jeybnmpr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ozkczlew.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3erjocyis.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3yocnexlz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qnlpathn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3odtuatez.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wvpgzrit.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3krfholkj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bzcbipep.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hrdkkcmj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cfhccjfd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3idmbafrf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jqnlkjhs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qlcgrzby.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fcphwapi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3frouuvjs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ghohfjqg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mmhxjqsm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bvhnkxmo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gbdnwlpp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lupvmwec.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gqussnvb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3joayzzam.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wzpwvrne.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gpteitxh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cszoniju.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hzrsahap.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cjqsrtgp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qwdqaumg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wucoufnj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3coytbvyi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cgoldeav.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nrwnbnim.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tyfxqbrk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fmtopbwm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3shkpfmnz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rcrmqyso.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3aqzeprhl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzntwzso.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hycdezug.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lkzmllbm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zbdrqdsp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yczutalt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xwoykrxz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vkptnael.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ahhvwrgc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cwfynkig.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxsdjjh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3aeccogut.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3siytqoao.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kweyfsdj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jkdogehk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bvbwldix.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zqxbpuxr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dhtizlmb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pkeurnna.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ibjrtcaz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lvhfodcx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fxdpalsc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hvwedtvi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mmuvipcd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fuxmwckn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bldwmmfr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pukevbvi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rlbdnqcy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3idcytglr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xtrfyzak.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zvfccmnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbkhgrdd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3itxnsalg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnftdztk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3igvrzzcb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xnxjbaxj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rdpfnhbe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bwoqvpid.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfaduuxm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3egsemixc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zshzbagv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yumfqoia.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tpvlclrh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3eyshacwa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3brdhujtj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fynuhglk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wjeavfvu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3frthrjay.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ibsznioj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bykdvvpf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dpikcroa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pctadvcr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3novogktl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uegzpjci.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gepmxeko.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xbsyjwam.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cxqpmipq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yifrpnsu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bqkedtpe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sqnlrtnt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hlydruer.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ohqjvfkb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mgnqtcrx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3taeossil.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hzthmxnj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3apboxwqs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yhycysws.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lnidfumw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3maxkceov.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ebtoblxm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rryhhjxz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3naloqhuk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3shcwdnza.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3amzmjxvw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwpxgvgf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rdoqonki.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpzpfhjt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ofsafdjj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yjvanxnx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ldcffxsi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3poulawen.html


<!-- 参考信息 -->