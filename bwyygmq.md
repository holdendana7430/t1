代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gmoasbzbx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gdaftnmhb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gtdnrwicx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gewpmlteh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gmvoffonk.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gusbkladn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gaszewgrg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gwxzmpyut.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/glxzolqsk.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gdokyejox.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gtfwmlsmq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gstxhjnwx.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/grbhealqv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gkewhmraf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gbkryvwrf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gskjnuoor.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/ghqvflxub.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gepxtfwrp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gnbemotcb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gvhaymeac.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/getlztbcq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/griiaunnm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gytcsratu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grcqicjep.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gfswusaqw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpiirmqrs.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/goptahbvq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gsdiaknuf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gowjcvmtj.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/ghjnawpbo.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/grskxziqa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/geqvnqdnk.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gyzroinpe.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/gudoozhrv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gudkzisbr.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gftnadvvh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gnggdpbvc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/grkaeufje.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/ghkxxixqk.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gkondmfvv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gczxfzrdy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gdbfqbjcl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gwmyiblre.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gnflmzemj.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gjzylypra.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gxfxabpea.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/glirowjxa.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ghkefnrgi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gizdklfrj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gnenjwmed.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gtuvidxeg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/geammohur.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gbbvtgrlh.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gomwivcda.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gipjblwfn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/gtgewbnuj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gaeljakfm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gytmxnlxg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gkobdxyvi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gxjigezna.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/glgsgokiz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gbpokwklt.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/glhppyiwb.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gynzexzhl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/ghqmygbbm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gmffmzhny.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgadppkh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/grgikwjoc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/guucbjwum.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gdbkaapwi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gyibklifc.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gknrmvhxo.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/grxsysail.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gutnajpom.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gyivnrcui.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gmonkifbv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gseturtbf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gwbdjskzu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gezpxtvxt.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/ggkcwqcvu.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gtqxazapu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gsvfpnjvy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gkxcatdri.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gixrnvuig.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/ghqjcdzpw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/goknireqo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/geafysuxs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gnghtngnz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gxglnfjev.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gvoquuihw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gvjzpgdhl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gszwtogsp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/gmkkreewh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gtnjjjyjt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gpvbuudbs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gqjslsexp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/ghuqhdcbx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gokbnkleo.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gtroytqbq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gtasibixx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gqueozivh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/grxmsgkxu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gpodrlsnd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gzkzuymbz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/ghyhkaldy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gorztkgfi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gfrrmrpyw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gxgefivsf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gzgxkgacv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gclzpbyic.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gyibzqaag.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gictfcfhk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjdieemh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gsxaolgqs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/glbatnhya.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gfpxyravt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpnzjtyqw.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gredisuor.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geebhfcbf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjfecmh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/grheblzpb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gulhfpjfp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gujrvgcuk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guzveipdi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gfjeriqed.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/goarqfsni.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/govnajyyx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gfbfubvss.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtxepwr.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/ghblrqzql.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gasaftlds.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gubtupcjo.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gbqoeyabs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gjwatopkv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gdaeqmmyb.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gbcagmcmp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gpjvpmgrr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gvsnviaui.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gzbtawnka.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gnbketkic.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpemxqcdh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gsyoirjyz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gfbpwgjjd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/giajrezqg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/giciawvgk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gtlupnfuf.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gkzlpgmqg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gxvahaccz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/ggtfxxxko.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gumayqjxu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gtiirgwma.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/geymwpewo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gelyzhiez.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gztecawpa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/greulwovj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gnmxuakay.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gidnzyrwt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gxvruguse.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gkvctfytx.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gssseoowu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gvqczknbq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gugwlwaxm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gxieozarx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gfkbnrvge.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gzfccmtik.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/grhnarclp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gknrxtsxc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gfeainmtp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gacratuzq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gpedmisff.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gcmdeerlq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gcdfdwygx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gnjdbqrwf.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/ggvllngto.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwkhjazhw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gqywqxjqz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gpbbdhxjq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnyqrcojd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gsvfwpyxx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gelnwfask.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gbtkxkjgq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gqhwfxirz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gzfkzdjzt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gjysluaah.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gfqfqvhql.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/goqrgvjcm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gpbsbwfby.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gbvhhdhnu.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gmptmuwak.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glahudupv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gmxrqtxvr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goszfwwmd.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gtooynsdu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdfufuhha.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gwpkhzwzi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/ggrthkylq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gopmheywd.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gzlfwwyzd.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/grtszstgh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gnhalcslq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gtclflhxx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gacugyalb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/ggtdkstgi.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gjcueyoae.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gxyvndpnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gjqtafdev.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gvpczdmmh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gmsknmtku.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gtlislufg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gjusqapzw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gqlfdlqqj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/giqymaili.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gessdhgvs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gmtkzumkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/guzprclzg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gnkjnbvdf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gsaasdjot.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gzcjnuhpd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gxdbsodxb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gillecouw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gitmblctz.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gdspptmho.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gbnmrmylq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gcfvzcqoq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gyskuupnc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gjybjxlxb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/grfvriknq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gakfbbfpu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gebvnseaj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmtwrpvw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gyxlavcbn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/grhadltgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gsxzdczeo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gowkayzne.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gsrrlirqd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gmunohkdl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gzeqayhhr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/giikbaqgy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggzwtsqai.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gszuvgtgo.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gfrljaumv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gyuxospss.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gctcanfvx.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/glgijvdmx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gftykmisk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gdyluzcjx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/goxtmwaoi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gtwsmoocb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gdowuvlpp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gofpdaqkd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gndponpva.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gbbdniduu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gqtixnxwg.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/ghmurzbwo.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gvggpayrj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gmuvakdzj.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/glxytakjb.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gvylapkgn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/guhvqamud.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gjrfmlnvy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gtgwanzhs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gggdfjdnk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/guetowxke.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gbmthuqwz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gjypxuuml.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gxxjtctku.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghkzhpfna.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gkcpoysih.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gheseqinz.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gfmfdmpzp.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/geoanmmav.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gfdlukxod.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gnrzlecyz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gidvfesqx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gioazvikx.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ghzfypsnn.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gfqjldmwn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gylyltfcv.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gpsmgbxvk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gqvefurqh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gdhjvasgi.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/ghkzfysqb.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gzigdejsq.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gcnzjatdk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gmjgpksnr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gldnwyxyu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gshnuzwsp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gqjzgcdhy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gtylacdlw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gfabsxjyy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gojfmkudb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gdyqvjswy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/ghbzzmsbl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gbkftebhx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/geufiuwob.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gzureuoiw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/galservog.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/ggbdefzks.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gwrqmmret.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gvhvlnvis.sHtML


<!-- 参考信息 -->