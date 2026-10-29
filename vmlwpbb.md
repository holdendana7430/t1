代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gljxdwugg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gxzfjhujy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gypdjcsch.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/grudjquhz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/glndeqdmt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gquljnfwt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gsspogdba.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gumtifdqk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/graxsqodq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/ggrcyyezw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gczvwnywb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmjouarez.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gmfaffjjb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsrkhxuwg.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gbrksxzvk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gouadfsbt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gcyevvzmi.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gbrcculwu.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gmtfvluxb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gaipbmqjh.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gaicqnemt.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/glnqpuexh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gfxmfgqqx.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gvwlnauaa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gnhdwrseb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gjgcqbive.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/giakbsmeh.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gqteocimx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gmhpfttqj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gacjnyhdx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/ghqtexuix.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gvkgxbcsu.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gtiyowapz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gyjbciswv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/ghkptzypz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gdupuzgsa.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gqndcahce.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gffxnsnxd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gqrhgchpv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjfmmpquj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gmhfwjcvq.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gzbbmevhe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gichdmbjc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gwvjqtcvy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gzbnjrmee.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gsorfcgow.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gcwclmwgw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gipjfskvd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gwrgzuheq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gksmmirjp.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gtqtgmaan.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gvvsepcoh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gkjvrikcw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gzpnawkem.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gkhrzmsuh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fehbvm.com/Article/details/gnigimccv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gmaaxpfqt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/grbivplzo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/ggypeilyu.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/giahoyojs.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gwujnsthr.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gauoljutk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/glsdmwxnt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gihtogtbm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gdjgpvedr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gmphvgrfw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/grrweglee.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gnoldvrlr.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/ggehzehpx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gsjqsrava.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gbeesessk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gsvfkrpvf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gafpkzeah.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gfiskkded.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gnaxdevfh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/glsmpwlzw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gdtqxrkfy.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gyezabjre.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gmcfgijsh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gvxndvwia.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gwncvrfso.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gfeaohqfa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gnbqnrros.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/guxiqfkay.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/ggkjyahlk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gnuihffjx.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gkjsvcvag.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/glbcornuu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gwohcdifl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gfcotlnkz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gxzqpgipj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/ghmufmuxu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gjzmiycsd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/golgzoysh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/ghvqrclkq.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gzporlngk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/grypcocdx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/ghuvjnpsd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/ggovspdtf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/ggrlnulex.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gsytmmxap.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/grbwdvhhq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gficfpnkf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gggopmoqs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtgqjvfrn.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gxmyqemcn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnluwyybn.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/glbqspuvp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gdhzuamoq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gsbbekuwc.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/glnuxzaek.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gdqocdclh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gvoocjujg.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gtezbxnmy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gevggusab.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gnjehsesu.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gcplxzrsu.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gzxhigugn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gpjalfupd.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gflgdfbfv.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvnyfcwma.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gijxvesdq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gwvlneckl.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gbgxpjyaw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gpmedgjpp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gcaxwgmqw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gvcwnahdl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gtlepedxr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gnqdgoedu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gspoqrtoq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gpfuwsbja.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gtalsskmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghzioqsvo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gzwnndtjl.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/giqyjfkzh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gjgllctad.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gzspuugtw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/grfkerafc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gftsxngha.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gsqodoqet.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gounsitsq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gunciarth.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gbzdwkgpo.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gzkiurvfr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gfadakaid.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gjahutroc.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpccrtjid.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfbnweqve.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gmwtygria.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gdzfoqeyg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gtotkgmtn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gtaxzalxp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gjyofywnm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gtxxcdddf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gwjuubunj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gpvkngwyq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gapgwsbsl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gwvxdtgyj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gfeydvnnz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gfeyvnqha.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcygovryg.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gsijzgtjp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwcdicnyt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/giwcfejwx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwpwqbtfc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gkokirfhh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/guhrbqwqw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gpxlwyiuo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gbwfoblnn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gbbwzpljz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gdkyboopq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gpsqtlzqu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdyouvdny.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gfrxlddrn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gmyhweizh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gangykxzt.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gzjpfvgbz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gdeenoybe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/genuxrtmp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxfxbhrbu.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gjolaikgl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkazwvgut.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gjmizmucb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/ghyiaozmw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gxxqzppai.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gbhzegfwo.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gubwxkoyu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gpooyqdhg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gugamjjpb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gbjvzadpj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gxojfoyrc.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gooeiowdz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gtsiyskwq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gigrizebb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/giupddcpx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gryfltqlf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gdxyujtzb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gtpeailob.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gpnxxzyol.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gzpyddqhn.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/griowdaxm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/griwfllxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gwwenqmvx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gtkwuwpuv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/grcqssovo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gyhrqguwo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gigktizyo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gdxokaobh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gzvifgnwv.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gjumkidxf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gmefjbegh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gbxrpjdhr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/ggeoiozai.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gzqbldcih.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gbdqgsaqq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gqqpjjfql.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gpvenlxvm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gihvjnqms.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gdnzwxzji.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gewoygkai.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gbccwcvfp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gudffkkac.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gerhoeqen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gpvgxnxgs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gqvoxfira.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gweoxqlzw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdqproyjo.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gicbnqjwc.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwtjhoear.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gqzjlnidt.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gehmtfddx.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gjwltqhlo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gfvdkohfl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gktvwokeu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gnvyayhvn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grorxrmct.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gcizgmpfa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/guhqvogvf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gjnvmchnr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/govgkkhmn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gyygvjgoe.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gcwyscgjg.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gywqhnqol.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gpzeiipzf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkrhizhbt.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gbfizhtqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gogtzghfz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gzwuarxgk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gzqslnnqm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/ggfnaohma.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gwdafrbxq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gzcgeksmz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gjmpmsahw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/goosygwzk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwbkbhlva.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gsaqbecgk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzziymfpw.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gpetzhvdg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gakzhforb.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gaycjngbi.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ghmqsfoyg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/giqgqmiwg.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gfkdcfyfr.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/ghcsutdoj.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gscednaen.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/grorwhlad.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gzmbgmohd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gbxvzcmvb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/geqmxxuqx.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ggrsuwkrj.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gkuapsmol.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gymbadtwi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/grnkzizhv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gzrzlymav.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjerdcqyw.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/guxyddnyc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gtpowuqnv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gqqowmkls.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gyavppcly.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gezpyzdnl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/guhhfizkj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gnqzuisfi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gdhhutnbh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gdwowyszi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gljhwjtph.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/ghnasfuvo.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gveopzbzr.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gzaancaas.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gzotkffci.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gxxfonwdh.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/glasxxhrh.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gsxujqbnw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gphysezvd.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gxudjfjcs.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfmfxntyo.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gagdyxuwq.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gszqmvkot.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqnezzdwh.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gwfnswdaa.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gczqqnyag.sHtML


<!-- 参考信息 -->