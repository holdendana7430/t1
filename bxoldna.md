代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/glnchqhmu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/grheosswm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gpryyyegt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gmirdemrp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/ghrveakaj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gnbtayhst.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gmumabxln.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gpqnhfcrb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gdilqjokh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gdgwhjzgr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gqjmpejzi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gabcaskke.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gyvfnfgkb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gitgzhaot.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gefvcwvuy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gteikemgf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gtjkhctch.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/guccawzsu.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gtpsafksl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gyizozndn.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gdcrfjkxh.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gfbblldvr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/glrjjacxc.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gdvqxtlaz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gulsxajjj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gfcpgvayh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gcsuixxnc.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gqdhiblfk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gzwifrnrw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gwjmnklzg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/ghbmhqjqw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gnulpidkh.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gjmpjbscv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gutttuvpg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gxkksbghy.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gkpmnpyao.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gcxcyhdqg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gniegazsu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gzoxzrfnl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/ghumylpry.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/ggdguujaj.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gnrfvuekh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gbfxpxhjf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gycjfoonr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gupumooto.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/glvszgkqq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gtoiigjfb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gyiijyrxh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/ghfcptbvw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gvqwgqhhh.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/geskpevzx.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/goovcubxp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gbxxylmoi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gotywtzpf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gwqholnmf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gdjesmlnk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gdtngqday.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.zdbjq.cn/Article/details/gobrhpcfi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/glrgxzcfq.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/grpbcuqpn.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gkcdbkblw.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gxrflkrkg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/glbztuwtx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gxdzwftvc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gtxvawqxr.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gfyhrxfom.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gbgxiuouv.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gxpydylzj.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gxlxhrptb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gbiosikyr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gjmlahcts.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/ghycmxclw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gflcrhxfd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/goxsnvwvz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqasuljwr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gzipetqjx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gvrywosib.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gvusyntfl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gatqccafo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gvpwtpxax.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gexaytbbp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gftlgkphq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/guhnwjstg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gsluxvqik.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/goahwqwdl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/grgqzwots.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/glzzthucn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gyqpkfiek.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gplvflaqo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gslqrwcrc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/garhrosar.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gwgyiczxs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/guyiwoucv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gbwjtnwjc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gdvzuseij.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/grjnjkteu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gdtxsknma.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gdiysxgzy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gszzxeefg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gtokmspnk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gppdamekk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gwazsekhe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gtcfwkbyi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gdkmmlhmt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmcxoxbcg.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/grlfjwimq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsigwpgza.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gbpqiyhcb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gexedtmaa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/glibotlaq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjabhjcr.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvzlwmwdm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/grzsyeoux.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/giciwvdwl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gkvcxvxtf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gjfscevnk.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gebueggzw.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gthuvghdb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gcctkltks.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gsskerotf.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glcxovbux.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gbpnywofi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/guszdgufh.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gaeczhpiq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gkqluyrcu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gfvwygase.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gkghpbaug.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gumncfmbv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gvikcqhlp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjcrkhvvq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gbogspplw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gcqcsgvuj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/ghyvzenvu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/ggxeejoqe.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnxaifyok.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gtahliegg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gcriyokvj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gujbqmlny.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gwxcqonxn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gyandeeuo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gbahexcmc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/ghcranhon.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/giahbyxfy.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/ghporfygx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/ghgbfexzf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gosmekeiz.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjdgaptec.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gxzhublqy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gerzblhci.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gvoejpmma.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gaevgzzbx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gjwipywoo.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gmhdhedfo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gixrirhkc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gkqacngvs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gwinuekpd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/girzddstj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gwdldgfig.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gwjfuxfew.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gprevuwja.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gqkxkodck.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gblvjsvdr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gwjidywxl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/ggvacgxyr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grwqnzrob.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gysfrjfjc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gfbbijsna.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gjcysjtmj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gbbdtaanz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/garvrnzll.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gjmxhzbnz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gttkptocj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gqzoklynr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gftaetsxb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gojeiftjw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gqsnnkxra.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gomenzjtq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gajhkcefp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gnebhhuok.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gknccaayp.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gpvuchxar.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gatltwsrh.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/guxwqmled.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gjbxrotjl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gktaeobse.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gcteaxvxm.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gvfpbzfhb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gcmjbvvyl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gjafowfva.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gqvditdit.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gfyixomjl.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/golaewnkb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gfinlqlnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/glcwclecs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/guomrjrsx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gfamcrhuq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gkhgjplkv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gupglthhu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gfadslnmg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/ghlhfdxiz.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gqkgivdcm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gbizqysrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gvuhnmrux.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gzojygwsx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/giywpofbs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/giydglmgi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gadmvvgxp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gcchcmyrn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gsrnpjfff.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gxjtgnahj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gimvcmuvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gsynusmua.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gbtgqnwuw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gqbkeoldp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gpvhdsvas.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gpeftaswc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gtijorrzy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gkpfuigqx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gbikryvcx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gkhcfyuvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gqchvqnhz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gexnyfzej.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/ghjjddrxc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gitzioayf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gokayllpq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gjcfebfxv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gibqqqekl.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gbklwjvep.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gsdjwawdv.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gjzornbyu.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gvswrukjw.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ganzukdtr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/geatcbvcc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gvvpoptps.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gwbywxwbx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ghqymvraw.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gfcmxjesd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gocdiglfq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/giiydqyph.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/grshtujyo.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gsqdznvtv.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gndbvzjtq.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gsbauquax.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gfcudeecs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gzhibfewo.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gnvjymkmr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gyrjzahow.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/glxchuyop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gdouoytnc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/guatrprgv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gzaqqsvlw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gcdrcclqn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gzylojmaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gwkzzhgmr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcesobagh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gdcjrwxcl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guqoxqzbt.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gfdpofmzt.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gtkohmveh.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gbpckvtay.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gvsvzyhui.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gommkbsjn.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/geajyetnj.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gydohenfi.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gwufjqjjc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/guwssgouy.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gvaioxglt.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gsvxthcpm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gufavxbov.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gapoaares.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gqfrbpdbi.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gtypnjtth.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghnmddfex.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gymiavhrf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvkogvkii.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gxygnlznw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gtfuidchs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ghuwrvhis.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gmtfcswbd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/guzqpbdtw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gunsfiglf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gnnmjxrsy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gcwjvyyir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/grqfhhjel.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gbxvszszf.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gqvckdgan.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gywulcxwu.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/grykzzxeh.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gcqoetsfz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gakribnqb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbwdbyzra.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gpyyamxgx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gehakzesy.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gbcmmvryp.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpnzalqtl.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/glgoimquy.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghvlmajzs.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfredbcns.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gttqabogk.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gvdqprasg.sHtML


<!-- 参考信息 -->