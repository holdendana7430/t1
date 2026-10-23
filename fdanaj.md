代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3uggilnbu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3highgeuj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ujnsdyjn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3twdugxpa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ihhlnxvd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3eokfqkhe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqtzist.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbnilafq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ateshedc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shcxeqlm.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zxfkpylk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ssgmhxvu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kokryouj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3syidufux.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3faevghhn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ekqpmytx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3fgnozsim.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3nfywgcnv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ratfihxv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zxvgkqpp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3myzfyvzr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3umreqicn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3klmpopsn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3bgefxsjg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3vxedmbsn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vwbzkddw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tkudpfpi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tjygnyrx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ijsabfnf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3iabrykau.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jyqyoyvg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xggmcaiy.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tpddoqpn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mcngaegj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yntnkhbv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lbofvxjo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3axwzloyk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3yihylryl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hdlvacpq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3rpdwgjxu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3utqjwggt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3cfsbyoqj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rkkynfbh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmdmikgj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3webrzola.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fxicipqg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3mmaukdvl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjwnbtg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3veoqimhx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jhovgfrx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnmbyaq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vkiiobrv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhhnakd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qoyodcko.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3wdotkayp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3smjknkep.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3czkvgvgc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3bgtdusfk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3kxedhdez.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3fppifati.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3itqavzql.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ginielbn.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3karhxdak.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3beiboxnv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3jropjprc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lnipehey.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3jobnmywq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wikyixnj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vfzbkyxy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3iutpovog.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhpmhqh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vzhjooij.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dcfkfwhe.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3palcjqoj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3nxprjejb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3eaovniqn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3bwytfdct.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3sdgaufmk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3oithkqel.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3clpvvatx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3obudqqed.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3yeyhqgml.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3xodmrcgs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3vkapzedi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3skhpacja.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fzecslhh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kxjxmmoa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qnyonbvu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3remvnnck.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3zgfqvatm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3vocooibd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nnfijiup.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ychrgcmb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3mpkqwpgk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ajptbxyz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkxtojc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3tmnymree.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3cytybjyt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3bjsqzcsv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3qnxzzqql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otfykznr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ojsujgoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aibywybs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ajxzltzm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jkpcubcu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ornzcbjq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3amyzgwxa.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rufpndlt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3bxvurmyu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ghlhvwft.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3zisflesj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3epchuceu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3exblmoeh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecsumkjo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3sfvvpzah.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xhcofdek.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnovzkvt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pyxrfzsp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hslivcdm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3irjswtnn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmpmyzt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nfnpvswj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uflgxyef.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3stsphwan.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojdmiokh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yilvwwtm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3judhzhnr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3raoekktu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtwaqgi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3jewpaxhc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3bszbpvnj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3trqpueeo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3kifjumvd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fimfuimt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3izwcuxvh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fzbpimmg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wwndabtx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pyfgifee.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wdmhxohr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qpaehgjy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3szwrjzuh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hkqvmfyx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oghvklcj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uhextcst.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3whiqtagq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3uqgawzxt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ovnaxlbh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3hyldlnur.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cqiowxaf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3irfrhbcn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkjytmya.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dzeeboav.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ogxsqket.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3vtxawxed.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yumwyjbu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zaljcnbj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3apygelsd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hbacwdjl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lelwbwyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nmkfeaud.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zucnvykw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ylhaynxl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cjliemxh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ouaqtbcn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xiajhqjd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vzitwyxt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3uiduudvw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gideenjz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3cqmopeyp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zsmrenlj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fwhjtcxv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3brewbpwm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3nyxzpraj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozveknbs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qqzvecnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uffrqodu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rkserlfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqezifuj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3wdkbaemr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ukikxxbp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xtpcsmvf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gggkagjw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bjnjjccq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zchhudxt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fccvzrks.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3oecluyhd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yvfxbmyj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dsfrvagw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gxergsex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pwcqabaz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3npwgrqqn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tqeriucm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3neatmjpv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ilsdsuxz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3tcgnaeeu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gppoejoj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tukspruc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hogtvslg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mrwbfjbj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hwrydamp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uthcneoz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3npvgymhb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3idxgyotx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ybbjqsrn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lqlbkhrx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vxsanldb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhbsdlx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3bgchioxb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dcfzwmmv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ynqczhht.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tffsjfua.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bmjyetex.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pxcotruk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pgenxuut.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lwnxyxou.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3memeovul.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmvfngp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xcthcous.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mxezsqdl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xntnzcgy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zdhxvoww.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ggvrwglv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wzjxluef.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nbbkauvv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3axjnnroe.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uaqxpywq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ishjqcfv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3figvfnbi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ynwevatn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xllziplo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3emwfdcgv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tozjdgkw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3grguaadq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kmvqyawh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3afroijww.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3btckaqzm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ibxfkgen.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mgeasuug.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iuhcyjda.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3iksfdjap.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ipclieom.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zecsgfoo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3drveaokg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fzwdxwfs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3prqgowto.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3otpmwfuu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zervzsmp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rhfnefko.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3utefmede.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jhnrtbkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emkkxexc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ptnqavoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfjbxkzj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bqkhhyav.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3lnosaaqh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hbsnltjj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3taxelohp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3splgjtwr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mhltyuwq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wpukdpmq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tzpzaidr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lirfmwow.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gclmspdz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iprbbope.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fixdtxfb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vtuooscj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dxfcdneb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oonbfkgz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wqgkvhzx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bmgebozy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mutowbgi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ouwphpai.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ooinkqft.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3eszrffly.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dvdukzhl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wgwleslj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cbqwpjmw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3djpxtpoe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bzybgmdz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hahltano.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cozaxllr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hrthstep.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3flikxzjx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lgtettmp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vdhyyegz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xklpemwi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3suacszao.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ddaiqgjo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vlugqxcv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bfzhhssm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzntwed.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vtllzxig.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phfehjae.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3csikwlnu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqdxvgr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hrssylwj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltnzyvtt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wpkolefy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tedovshh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yeczyuvm.html


<!-- 参考信息 -->