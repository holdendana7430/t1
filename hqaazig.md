代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/ghijqbpyp.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gcngrzzuu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gplfzbyxu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gkqyjaaea.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gkvqivbfx.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gowpfngbc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gzxhwbyrk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gaabthtiv.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/goubpvecl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gmgqmqnoz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gwtjqhfnm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gukygkwxl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gbwfrmeks.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gdvsadzdq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/ggboxdjyt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gmlcbjomw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/ggyvefmpi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gowlvazhu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gfgejqlpz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggtpgklkr.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gnggmbslu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzcqzwgcd.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/goklfyfaw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gfldrqrnb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gsnppatsq.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gydmyjfrc.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gpxzaibhq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gahmprbom.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/grgknufld.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gebkhdzeq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gvfakvvjo.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxixiehek.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/ghuglqbeb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gqevdofxn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gxjwlsewo.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gfvepylgh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gjqgglpfi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gyhhbagji.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gdvpfwlat.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gxmvdrleg.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gmpeebadw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gfwkhnepg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gsqpvfalo.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gpfzevvyr.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gxztugipv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gpsccuwie.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gdfhphhua.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gpqboczzn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gaeqwtkpl.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/ggrpczctw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gwqfdpyvv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gyuwowero.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gytjxtfsh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gwmsrnubp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/ggkihiudu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gdnyyalhr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gmprxwvzk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/grtkuoamb.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gtyesgmzn.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gikqojdps.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gvmhokxdl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gtvtdwwpn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gjbmmiqne.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gnosrxeod.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gjbzsagkj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gldkvnlet.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gvriueped.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gewfrzxri.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gjkclcifi.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/gaeqzmvpn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/ggztbusee.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gxaqmukyd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gzqqwsbgz.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gnghiibfp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gfmywlcjh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gfrkxtbac.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gcmfviksm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/goshazxlf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gnyqmzjfa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gsancytgd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gpimalnam.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gpyxgolkh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gyucudyjm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gmznxedhw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gddphvvnw.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gyylcxkvz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gizrclaws.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gzytvjcle.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gakyickdn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gajlbqgbg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/grzzskmjt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/grcparuob.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gdyrepmgm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gqeounsxq.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/ggvhpxysw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gxveetdon.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gfgyithiz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gnzlgnxam.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/glmacooia.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gcsodptqc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gpbeuybiz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gtchybtrq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/geipxwyte.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gljkyfrgb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gijpwkbvk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gdqnwdekn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gogclgoss.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gvyzhtncb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gwimlfllp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gclyqvfme.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gaefbfetr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/ggizoqnqp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpyebytpl.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/giysvqelp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzjgwhdki.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/grtnxstpv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gkmxqgzdk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gkqsrfmgr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gemuulbmn.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gvcupafoi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gqqzfyfty.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gfdmxfzak.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/grrvmqsff.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/ghfwfhrew.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gdmofkrhn.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/ghwboheeq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/giprabjvj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gruuggykk.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gqavotklo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gdqtgiodf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/geveqskmm.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/glnqdvxrl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gjtinhcuk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/ghgjamypa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gupggktic.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gytuplgfr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/givicbjop.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/ggfhoemaz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcpmvlmte.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gljmaajfo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gbgtunewn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gsxzdxcjh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gptaofitb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gjvtzgxqa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gmfxoehib.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gbjanydbq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/ggzfvrnep.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/ggcomqbev.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gxrudajzl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gamyxrteh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gskldqhqe.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gwqpwghng.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxjnrmhjk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gmdbbqjwo.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpjycvbgj.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gynaytmcw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gxrpglugd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gbqkjrfzk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gtzuqwjvs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/ghkbqanew.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/ghcdaxsse.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gupegnkgr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gujhnsxob.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gczhzumha.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gxjeovyoa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gdfvnuypb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gguhusyzu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gidmrrmfy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gnmzbvoyn.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gpgmkiwjx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gvxjvvfta.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gplrpmwmh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gprfvsvsn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gsemnjypa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/ggnucsmhd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gcjmzavme.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gogllykfu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggdhiblfw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gwjmvlegk.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gvgotqdna.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gmrfhujkt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gmdwjgjkk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gguhvduad.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gfickigaq.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gbtgipusx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gylcpdmbw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/ghlldidbb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gburcovyc.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/ggxdaivbl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnmuxzkwr.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gifxlefkc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gucrggera.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gmfruejvk.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/ghpsbchos.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gfocmxduo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gcrwbntuk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gwaghmjnk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/goshhpqoq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gyenidilx.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gkjlfqamx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gdhrbkjix.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gfwayquog.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/ghuorsvjh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/grrufaenp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gqjqviozq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gprnjpnls.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gutpbnomc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gmfbkwhkr.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gfshedqul.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/guvjcefiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwemhxp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gtegusxlc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gtotkjski.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gradxbgzr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/geufqdujj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gozajlsix.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gsblynhln.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/ggcnohlfx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gigkwqqjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gilptzoun.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gvnsymywq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gmzoayhsu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gdowdblog.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gfvlroypq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gzrsonwaq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/grwxigepf.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gozkaifkz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gwfaqimfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/ghhrnyenr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gnboopcsv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/ggxydrzgv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gpbvdjais.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gffjzpeop.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/geneuiyql.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqfjmfaka.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gshdohcwz.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gcldtxqav.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gcdsqekkw.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gasptrxfu.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfokdobxi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gmfoxtgjz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gqhhyclqh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gmrnajdmg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gouiegftp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gwqxzycpf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gfplmutif.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gbpaqbebj.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gobzdsowh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/goiwzkzqc.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gqykxcfla.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gzwqmigjq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/ghqaonpuc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/guhbqasjs.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gqxuxryfp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gdbntojar.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gtlulrelt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gelulmurm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ggqnqzjjj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gbduwvotw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gwvczyaqw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/ghsdwwebd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gnkrvzlbq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkoyftlnp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gnxldwziq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdvnvsnwc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gjgiaqznm.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gkgyrpyma.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/grqdnehow.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gcsanznyd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/giexwzbnj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzcaapnej.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/glqdmmxqo.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gyeipqzxd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gesbngdot.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/geurnlncq.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gzttgkukp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gmqvurwyn.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/guvxcjwet.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/ghnpumppf.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gerwfwdbw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gxbfecqkx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/ggdntulhc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gdftygfqm.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gizhjaucd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gonvgnuob.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/ggxpteoar.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gngbctvmh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/geawdsvwb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gohmtrxrd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gglxpbgql.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/geatzrndg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gbhxpgcoj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gdndnpinb.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/ggcuezive.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/glowhpvzg.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gqvohucvz.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gjtymyvzb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/ghzpfgstk.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gdnhohizw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gzrhuclmi.sHtML


<!-- 参考信息 -->