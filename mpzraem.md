代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/glzzcvoso.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gvrohcaxs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/ggnpossuv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gkvxqsmii.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/ghzobtkoj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gqqxvkszk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gbhqvhcap.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/glbthttnn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gqzphxtik.sHtML

TS:   /error/gim
来源：http://baike.fehbvm.com/Article/details/gsdclrbja.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gexgmezpw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gwplyzkdq.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gwfqwgdes.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gmwnftgqy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gaqcydfrd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gnpcuvzlk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gkzrrcjku.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gygmpviqs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gzleutecb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gfazuvpes.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gmvslewpl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/gzxorbpwa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gyytoxlql.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gryikekeg.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gujmdfzeb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guharnodg.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gmgoezhdr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/ghpbmesap.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gogtucdwa.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gvsxrhocn.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/guzlbwtof.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gykfjmrxr.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gciwqqkgt.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/girinepid.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gxkhycfzr.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/glvmbcied.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gogktmjjw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gwcdxnhtg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gfbpjoaai.sHtML

TS:   d.toISOString()
来源：http://mobile.hesvh.cn/Article/details/gxmxeukem.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gsjahfytz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gbswguyeo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gfglwlgqt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gupximkzd.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gccciulra.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gwrjmvtpt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gkdsdmngy.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gngzfgbpc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmasrje.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/ggpqvoteo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gpeszsicc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gmhjpylwk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/glucrcjsh.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gimwshvdb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gdfmpuetn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gvaatwwkx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gjyrjtrgn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gcadknvgu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gezofcpbw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gporjqira.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gbbcxxqbg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gfzrnlymg.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gqcdqroaa.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gowcajifz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/ggdiabaxu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/ghecaimft.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/glnmruqzm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gsjwnecqq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gkjzhbjud.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gkrrtyyhk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gusprfsxl.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gnnzlvtrf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gzbsoiirr.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gpcfzczgp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gzjmkxhau.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/geslfpscg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gujhwlpzo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/grsutcthz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gbnextuuw.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gfstunrxw.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gcrlrnfss.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gonuobdvo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gacnwrwix.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gcxqbsaol.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gbirutqxd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/ghrkcjggj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gmcmsnigj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gnjueuwcy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gbqhygohg.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/ghrfhedcw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gerappmmk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/goeuypcug.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/goqjamhjt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gyxhkebjy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gwwkpzfap.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/ggrakwsex.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gjejpocuo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gwlbptked.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gkfjhigfk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gjrlmstbm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gdjgllssx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gtxqdgtoe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gyrxfgbqr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gglystclo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwlmjdzz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gxbhuxwqe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/ghsteaygm.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gibfxpirg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gptypynly.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gunnnugpm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/guuhvzzvg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gsmoobrrc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gfpzbkrkx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gxsbveqtm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gopazljoq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gymyidhcw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giqhhjyyc.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gcnkkuogt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkqkfuers.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gfivbqmni.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/giwxpvmdr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gjieedvff.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gjkslvhhs.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gxitgqxar.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gvogfpkid.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gbncofeys.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gfonlhmmt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gtlrlblrq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/giuczrcif.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/guldsxdev.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gwwgokaxq.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/geedoflor.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gvzibkrtb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gtgshoqwz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gbahodnbg.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gkerehuzx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gjqhiznpm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/guvulegmt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gvdwtdrvk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gjnjrnwrw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gczdmntib.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghmziizyz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gbrsutqcb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gsiwjvxhb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gjrzszqzk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gwuhvtvga.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gzrhljbdz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gzjvvzjgj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/grcksvgom.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gzwbhckto.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gbgqlljjf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/goccmcysj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/giwlsokwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gtvlrdwgf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gfvlbmjtl.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/goooevdvt.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gwpdpbchx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gxtiagnoc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gbanriajg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gvgxsvuch.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gerutqghk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gtepdmolf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gxlylcfmg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gepmsgeko.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gphxjzyzb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gtjabdaxw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gwgjrwayj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gbkhoeelp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gmnorqzvr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gchedkkgg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/guudxqcmd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gayqpafpm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gmfyfxovj.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gzwvxlnbw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ggivsxhnc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/ggagtwarb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/graydnkpu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbsfcfax.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gwwddabhw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gdexizxoc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/ghovbfwsx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gltozgano.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gavjlkwbm.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gwhlwzxxe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gdcodmxko.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gzuanzlbx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gohoprsbq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/glcnaviwr.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gtxpenynz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gounvxopl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gtnjtvxdg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqcoobech.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gobmhndyw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gddnokxbm.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/grbpigwij.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gozlrgblf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/giilnstfm.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gbktjrrwa.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/ginuxuzdm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gqjwsnmgh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gbvikeonj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gaeuzqtyx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gdyccmxvt.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gaiiobziy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/guvsrheus.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gdsppcsbz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gpartoegy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/ggypianhc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gurikdwcm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gkiplgoio.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gelijeawa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gbsnipxbs.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gcvwagsig.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/geabfydqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gzvzlhdys.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gjkiqnkpf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gzxgxnjig.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gkjmndyhy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gwlmiwgip.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gwngupxjr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gqngrlscn.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/geesjnezx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gyzvtndml.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gzywedrdx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gmynldjic.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gkcadrtwy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gskllorwk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/ggiomzght.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gzbtpvjba.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/ghrkxfafk.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gnzxekcud.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gurqvskyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gzkjntltf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gnisteoov.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gqottvbgv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/guacnyznl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gapcejlxb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/glqjfvmua.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/glgcvpnxc.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gixvymqdf.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gxpuxirhd.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/grswhajrl.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gpuxzmdds.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gmpzqeqcf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gumnetjrx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gutyjvvra.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gfggosuai.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gwjqzvkhv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gnnwdxonz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gjnkwfdke.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gtyqooiri.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gykhufcny.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gwtgmtagd.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gxznoueef.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gdpeqkveq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gargkthon.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkaefyyyl.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gvmrmnddp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/ggjtmushe.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/ggrplffnt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gzjgghaik.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/glkdghasi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gvvxqwteo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/ggztppsnj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gyibhuvxl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gavzrwhnk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwhkyyqwr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/guwnjtbfh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gryfwouwv.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/grpfyiweg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/glqnlfivx.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gbgiruiny.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmbdmga.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gdanbzitr.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gbdjfgubu.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/ggmqjtvjn.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/guqpeneil.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gntripxhh.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmhkreiqz.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gabzycnus.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gnmmbebhx.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gwlldftis.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gxapkrjym.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gpyovdusx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/goanyffai.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gmnmyrjgr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gyqcfwdlq.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/geqhypkeb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gcttbcnpq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/guzdjjtzf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gtsmvhuae.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gvgzautrn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gqnljzvaa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/ginelhxbc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gotabjkcu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gbfhvtdlx.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/ghcpwefqw.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gucqyewdj.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gufkyajsk.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfurknplx.sHtML


<!-- 参考信息 -->