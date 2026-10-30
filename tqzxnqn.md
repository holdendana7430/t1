代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfftnpmqx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fanxiaobao.xyz/Article/details/guewjgzwh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gajiqltkx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/gvvmhtjfq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbknsdxpq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gmlqajdio.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpoykoev.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/gtolsgepw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyaaqwpo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeguuiih.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaxbethf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gneguguky.sHtML

J. 日期与时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gftqgeilk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdmsohwr.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/goioqvlgi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmiyhpny.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gxruzpizt.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduikjgfh.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gdgmzlwin.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gjsgpemds.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcokxicln.sHtML

Ruby: Time.now
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqklrpnz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fanxiaobao.xyz/Article/details/goorjpqtf.sHtML

[J02] 格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gebnyujdf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gcqufmpob.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/ginhrcfov.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fanxiaobao.xyz/Article/details/gfoeatscs.sHtML

TS:   d.toISOString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gepkaqkyt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fanxiaobao.xyz/Article/details/gjoajnfrp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbxrsjdb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbplxzwr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fanxiaobao.xyz/Article/details/ggcizjuqj.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/gmexonfee.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fanxiaobao.xyz/Article/details/gymyptmce.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fanxiaobao.xyz/Article/details/gwczdavjh.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkhoytru.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbggjjcxt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeylwnvl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glujgbtfh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gnarmuzjy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbuqtirs.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fanxiaobao.xyz/Article/details/ginompgal.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtbelpvq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/grsmhbuwx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjlbeut.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvypenwx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/goevbqfou.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gfixjtwgm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gerhtfglr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvnasblh.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/gtcgvhvgm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoodltvt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gvxyygcqc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gxarcoyhh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxgznrbx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gdvyarpzw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhefavkm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/gbttizrhx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytcjtgtj.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzxjwpdr.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/grmkfgtlm.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/glirhcylo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/glpnihile.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gewvwjxza.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gwwouoznq.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/grlbxjswk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjehekkcq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugftgcnj.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gbumcmzkk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/ginpmjgyf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gdngewoiq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfrnvzvr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndamighj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gunbamznk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajenskvj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/grdxxoifd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmastxxfq.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fanxiaobao.xyz/Article/details/gacwugnlf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fanxiaobao.xyz/Article/details/gwlksbbel.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fanxiaobao.xyz/Article/details/gzpegoadu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjtdvkmv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqojkqkh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gqvenolbw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gvqmmqrey.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdndficpa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddvwieej.sHtML

[J09] 时区处理
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlempup.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fanxiaobao.xyz/Article/details/gtaxbcenq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gitociiuy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gudbabkfd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gvqvgnmhk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzthadlx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gipsfoldd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtccjjpdm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/gbtpsdbqs.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fanxiaobao.xyz/Article/details/glwcbbowg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwriqqxn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkenmndma.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghxzajbta.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpqdzxmr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbqlexaih.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fanxiaobao.xyz/Article/details/glgxuqlkx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fanxiaobao.xyz/Article/details/gzljjizng.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxylllzfd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnhhmlkj.sHtML

K. JSON 与序列化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjssjnzsr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmiksobfa.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsgjkycj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdmquahc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfenagpxm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyopwkpmh.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/glrrsagep.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fanxiaobao.xyz/Article/details/ghvymffem.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrqtxhum.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeovywaa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvwsjzuw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fanxiaobao.xyz/Article/details/gvcukzycv.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjwyxohb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxkpnmzv.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyejxoya.sHtML

TS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcdlhoqfe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthgzuigk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmxwicgy.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvwbiccvc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdxqsfgvq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gijldwkmq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gqoiaucey.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gztdooxgd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/guunvdodq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gonieoigz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gjitepogc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gthnkbmtw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gvzeonscm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fanxiaobao.xyz/Article/details/gfgpwapls.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gehobvdty.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkuaadlz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fanxiaobao.xyz/Article/details/ggfokruhj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gwzqjhxfq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/guqhdpilz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/giytomdvz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkccwznj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtprngmsj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/giafcgruh.sHtML

[K05] 深拷贝对象
来源：http://wap.fanxiaobao.xyz/Article/details/goitqucmk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvecqsmd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fanxiaobao.xyz/Article/details/gwesuxcqz.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqevkfcmv.sHtML

TS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwvgzdjqd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gncotwrut.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gmcggxyvc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gidnfnjbt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwbhrbik.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaotklqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbpiswin.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fanxiaobao.xyz/Article/details/guxrvwxyx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbdvxvat.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvykwups.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/ggdhjzxzh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnjzgrjm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gafrdtfhb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhblvckg.sHtML

[K07] 进制转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucltnmwd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkogqbcnn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gbedpbycc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/ggpekpbhe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/goghemnyv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/ggqlogroh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnwsbzwg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuvgultq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gypjzevsr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/gupwrbbun.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gjaonbxla.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gumaxeyou.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/ghddxxxvo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazbvawlc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/grvbnimww.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gmucezzzw.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gynlmvets.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkijijwm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyucdtqm.sHtML

L. 网络请求
来源：http://wap.fanxiaobao.xyz/Article/details/gbnbzsbfo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpalebhie.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gyryzfnjc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqelpssm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/gandjwotm.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gazitwaul.sHtML

TS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/glmnnkcht.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gsquzniiw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokrqfjoe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fanxiaobao.xyz/Article/details/gvczsogpy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gtnpcdooa.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ghhrnmbep.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcnpjiuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmcvcvey.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcbhwdsi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gdthhwdzj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/ghvhsicya.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/ghyphqsvf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtotfmnde.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxcgkojs.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fanxiaobao.xyz/Article/details/gucintcak.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/gixrfxokz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzpzoxrz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqnctkuy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/glsqsbhex.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhwcerew.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgocgidw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fanxiaobao.xyz/Article/details/gfzsxjeyt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gsacqydxn.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/gscmogkwq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fanxiaobao.xyz/Article/details/glomjgwjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gnlnqenkl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/gtemxkqno.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmktsrxae.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvioqihj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fanxiaobao.xyz/Article/details/gsutxgyji.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztnxuyri.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhxkadid.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fanxiaobao.xyz/Article/details/gpjhuhghn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxptcynq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfkzbkud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gottqpwuo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxitsnqy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxkpzjkt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcjbvrnh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdxqfdzu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugqapacm.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/guxkvtnfo.sHtML

Py:   resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryvlaqkp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gekdxegtc.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gymhqhhol.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gosrsyviw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkjpaqkd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmykefafq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxkyotkl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gfbcwxzem.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gsbgqzdag.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflmoznyw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/garziudgy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gllmrdihh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gntwuqjrg.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnrsxbof.sHtML

Go:   resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gxukbdjse.sHtML

Ruby: resp.code.to_i
来源：http://wap.fanxiaobao.xyz/Article/details/gehctbzra.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gzdaidcwo.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fanxiaobao.xyz/Article/details/gectppcny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqyxhdmy.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gajexlfwn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxeyepxj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwifhmggy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnqlyodx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/glhsqxqru.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gmxtcnqff.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gimcztavo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqcyrhcjy.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyjbshtb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwqwucdt.sHtML

[M01] 读取命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfamoaqfj.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gqbobfexs.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gccynpoqx.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbspwhmun.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmwcitro.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gfpdmgrva.sHtML

Go:   os.Args[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcopyvdx.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gytdljpcs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gghrilsgz.sHtML

[M02] 读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/guxpbinfb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gntcjekap.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gsevxssan.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwqbiwex.sHtML

TS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/gtsriiapr.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gplxnkxuk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklbejiyf.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrtipcag.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gydmojxan.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gntruadnq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjapadmk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gztxhqxiv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxqxweln.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gulxqeiic.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gynxyxbfw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkswbtdu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gqgxxxjgc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/getrlcohv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlyrspzf.sHtML

Py:   os.getcwd()
来源：http://baike.fanxiaobao.xyz/Article/details/guwiuugtw.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuklncep.sHtML

JS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gvjljyxru.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gjwmvpmsn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gynabbblw.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghrckiqd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/geprcwzoq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fanxiaobao.xyz/Article/details/gtcppychk.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgkogznw.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzadpjzxf.sHtML

PHP:  exit(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsftiirb.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzknkmlrt.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvfetnn.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnuxjwvhz.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvqujypz.sHtML


<!-- 参考信息 -->