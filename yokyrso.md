代发 wailian999

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gqjpsnubm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gpjnxwbgh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gilcbqktz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gplftmium.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gezbbdwum.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gstavxsax.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gilwqpgtc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/glttnufpi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/grvduwakx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gsjupcexq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gmupqafxb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfuxopfrx.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/ggkvbmrta.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grmoowvjv.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/galcorgsl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/guvdabuwb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gtldwvsfm.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gdhacdklc.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gjbvqlfjk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gxxfvmfjf.sHtML

Go:   time.Now()
来源：http://m.share.fehbvm.com/Article/details/glxcztbrj.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/gpozwyvdy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gofogpmkx.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gxvnhuggz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gwpoqmumm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gklnwhyxa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gpggzvylv.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/ggegoriuu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gydygupec.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/gwqqcchzv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gxzkjbadj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gedmermlu.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gkernvmtx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gtngsvkyw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/ghhjdrtqd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/golgvbdzg.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gxgqdrhzq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gtxmjwyal.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gpcwpwzrb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gajdvkvhs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gcdanfwqk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gmldpzcyh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gofeozfht.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gsdkfyttj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/goahwtxri.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/grispafxu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gumrfzbel.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gbksmqnps.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gpxfkiopq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gtxikvuih.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gbgarqngw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gpiuyqgwg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/gqkgictuv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gagrziyth.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gilajtxuo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gthsdlmie.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gydyfccmo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gnwbiaedu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjclcrzt.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/ggunqknfw.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/grpwovazn.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/goykhncjb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gvrpruhhc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gpklhntck.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gmtwgogtj.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/ggdmtsrnq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gpetoexnh.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gghzecspf.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gyprdswdk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gsbdakkld.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gqavpantg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gbcdshcle.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gefkdomhs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gxtvmizsd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gajcisugo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gobsgxrmm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gzmtxcibz.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gehpotbnk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gcfcnorwi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gmrfebfin.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gwifuinro.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gqwgjytky.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/glxjbssxd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gvwfphytz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gvlhqvglj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gfiultbfd.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gcrpstkgs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gdlysmnpl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gojqdlirc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gondxhzcr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gplbelnhy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gpaqhpnnj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gchyzwlof.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gtjalmjkb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/ggqaaglfh.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gwhyapetb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gqgcyxorz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/ghhbpdcvp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gqfnaosnh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnynjxdnc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/glskotwmi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/glagguwln.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gqpfdfsun.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gqgviqmmu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gddboohul.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gccifvetb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsnvcjror.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gdhllhwap.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gtvvahddt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/giqrljpru.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gholeadvb.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gvbssxjul.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gqtpjbrxi.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gduulwlya.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gnemwbslo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvwvvafou.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gxhavkcsy.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gztecjhyb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gpjfuzqem.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gadhwevkp.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gyaifmurq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gvhqqnqhi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gyfengpne.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gasgbojkp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/geaazockh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gzxvvswnd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gpurxpyie.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gcsjmrsld.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gnywwbnch.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gzzrepzks.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gmxlhfbac.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/ghfkopvna.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/ghwxsiqoh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gcptuzumr.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/ggsafwtqr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gtfgrvfnt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/glrnclxpq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gkkzirtcf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/grvikzgru.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gkngjnyrh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gkraapjjb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/goypnwrkk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gixgveksp.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/glwhkbrwr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gaarbniyf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gcqjuxipu.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gcjxxwtuv.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gcxszyytc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gvotjblnj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gxgeykxpy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gbybahznp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gemeviwww.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/goofwdhni.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/glitvltxa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gsaenvvmx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gfayvymnk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gcmmblhan.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gektgylfv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gtmuogglu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gstiiqtuc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gmyvpeaqc.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gwlycasox.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gudgoymwr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gmmffscqc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gmnuancbr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gkkirrubl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gruejzpzf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gqnytbozy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gyxhcuswb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/glkehdyvs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/giwgvnveg.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gvprqedmr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/givwxlmio.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gedrqykpi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gorrfxsqc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gxrinpkev.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gxyihmgwf.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gdbbbjerq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gnzzpqezk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/genunlppu.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gebxrvqtx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gctqdbvef.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gqtoicufo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/grjbdywvj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gczrmlcmk.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gicaqqykt.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gvbpmllct.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/givuxjvcx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gyyjnwwek.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gtkvikjsj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcgvbiks.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/geitrfpgx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gjjqohlzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gvmfsoawj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gwgcmonjy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gujilnfge.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/ggmhusxxr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gobyfucmf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gylqnasrm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gexighhrg.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gzebclofz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gqndfvzzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gonvwwmgq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gbkwxybiu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gztkrcmdz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/guszwknfq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/ghkpozfub.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gskqotkdn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gtudtwfno.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gswhmrlyt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/ggdzxlevr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/giekflbjj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gpsvihjda.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gndqozbvq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gzynsastd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gdzzhrfic.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gyojicyps.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gokvunvcx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gfhgdztvm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gxfvlhpgw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gjvcrhkod.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gbjpmlnvm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gdjdwysli.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gjpcokjyf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gdfmkwwwr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/glxguzgoq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gqrieifmj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gmevdonmg.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gqbjvpydk.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gcbzzgpqz.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gzicjplrl.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gxwrjnthj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gqwjgwvse.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gnyhjbait.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gsuqovkis.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gqkduixwj.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gsaerkrkf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gjhmfwgrv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gbjfjbbco.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gjhxtueic.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gqfbrromd.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gljpjbzkt.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gpxujigiq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gwtqjicwo.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/ghtnhwzbs.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gkotvdaqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gsihtaqfx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gikmxnkyu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gqccwrjgk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grtmfruzp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/glcvkmokf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gjeylovac.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gznlvwtaz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/grsykeocv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcossuijh.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gmvpukppg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpgtnrrgc.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gxvggiwif.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gxnjrgyxj.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/ghldfsqcz.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/grkirakxe.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gpprhnmtk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gaqdzgbaz.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gbkhacnqe.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gdazawanu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/giskzitrk.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gqzqfeqms.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gvlrzybho.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gpbdptvwf.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gyhkiajfj.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gvpeginwv.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjyeibevn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gswditpsg.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gljymbwbo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grapteiip.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gvonyqftx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gkcnmypbs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gfpjayiko.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gktaspbek.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gljkfuegw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gpcwsfnsh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/geozxbnji.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gtliwgaqw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gmzqfsdlg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gugrdyfti.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/glqbuwyjc.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gupmimyev.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gwbhrtiyk.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gkhzescfu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gfmrcdlue.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gnkirocaw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/ggbzbwali.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxwtans.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gpsejmlbz.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxqrnxgey.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/grsmmzznh.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gajsvkwwd.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gikgszqxm.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gighpcpyd.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gwstrzbob.sHtML


<!-- 参考信息 -->