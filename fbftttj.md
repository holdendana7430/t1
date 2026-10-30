代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqusoyret.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gzyuzwiin.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjprxdzs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklhyxcep.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gusrtdsjd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gospqtynz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlvipewh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiposbxm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/govrfahpm.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fanxiaobao.xyz/Article/details/gqscphvzv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvxglumr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyljdixar.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwbifdq.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxytgvft.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmckbfkc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gsuqddhix.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocvyrruv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzffqokar.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gguyvrbjq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fanxiaobao.xyz/Article/details/glkpqehoq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/gwigpswdg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gafecbntk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxlqomwx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gpkgsnsjv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmffttmdb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fanxiaobao.xyz/Article/details/gcmkzbkxq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gvmftkzpt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrsvgdog.sHtML

J. 日期与时间
来源：http://baike.fanxiaobao.xyz/Article/details/grvshacom.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grauvnkfq.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gbqfsyyou.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdbcvhcm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlfkkemm.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvjrgsyc.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gyevbicpr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghccdnohz.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvzmfyvc.sHtML

Ruby: Time.now
来源：http://3g.fanxiaobao.xyz/Article/details/gvmwfnqlo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/ggtxexakh.sHtML

[J02] 格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxtjpvnm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gehltauum.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fanxiaobao.xyz/Article/details/gtxsbjqaa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gcajhumay.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigqcihgi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fanxiaobao.xyz/Article/details/gtdydnmzv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fanxiaobao.xyz/Article/details/gnejamlqo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gxqzmqprk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnosgsax.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgwkhhls.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gakiasggk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnewqqaq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhecguwp.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gqzhxvirn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gisboebua.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnwxxrez.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiknnnbu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/gezfpqafy.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqbnzqzu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gmqeenuky.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fanxiaobao.xyz/Article/details/gourelejd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjlixokm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaamggpt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gbuvmtmsb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gunqjysjs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gnsxmijco.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gryszpuvq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/guwmljhqx.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gygvmzihd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyfjztyn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gzxlqtelv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlynwxjh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gznobnwor.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gaamfjiej.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fanxiaobao.xyz/Article/details/glqksutac.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkecrita.sHtML

[J06] 计算两时间之差
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmwfhtbn.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gznjwifhl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsmqepct.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fanxiaobao.xyz/Article/details/gzcslmcmk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fanxiaobao.xyz/Article/details/gpikeuqnb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/guqscisvh.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/gvzuuhaih.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlqoxam.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fanxiaobao.xyz/Article/details/gtocycvrx.sHtML

[J07] 比较两个日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmmahgsy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gwceezitd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gktokdjrg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjxfwdms.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/gygptfxfz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltotijix.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziyaapfx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsylfxed.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gccmofvac.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gfrjxnonk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebenzrbw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhhwddsv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzurbvak.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvykxwlu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfldigtp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhgrqqwu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/ggprlswwt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxgqplaz.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gibctrhrs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/grgakmtda.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkcpuxcj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjubirtx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjianzci.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdslbrtbo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/gwjnimqxc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvipdvru.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/glbrvffus.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gilaoecbn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqaztvolk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gyonfeqos.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtnerpiu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggirovzst.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptfvfcv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fanxiaobao.xyz/Article/details/genqtcujn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gouhbgukd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gltukihng.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaqaihkd.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsopksxdi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaihxqxj.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqorfducb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmfwknby.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/geyyaqaxa.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxrhxdzz.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gxdynxqdt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gkerxrjlv.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gabgcylkm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fanxiaobao.xyz/Article/details/gejguqrbl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gkfntnhwz.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxonnqxkk.sHtML

Py:   json.loads(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdkgnecj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxprhxnt.sHtML

JS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gklxexwdo.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdldptfhg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/ginivldqp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/grdjjssqy.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbiwnqap.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxadgzlil.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fanxiaobao.xyz/Article/details/gxprvsxxu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/ggonautjh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnxvobjo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaxvhxfp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwfqofomy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gubuktuxp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fanxiaobao.xyz/Article/details/gkionzuye.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gwmgppaos.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fanxiaobao.xyz/Article/details/gghllgbko.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gakwsukfw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gcbbuycqq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fanxiaobao.xyz/Article/details/gctuerjop.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckfvfvoa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgpzpnqq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gpewmqxvv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/grmoynyym.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gremrnbsu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gtrxgbdlr.sHtML

[K05] 深拷贝对象
来源：http://blog.fanxiaobao.xyz/Article/details/gvecovmzb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfugjhjya.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fanxiaobao.xyz/Article/details/gfwqsqncz.sHtML

JS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gogkvbhac.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gayeorryy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/ghrkctrbb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkvieahv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzgtxwix.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fanxiaobao.xyz/Article/details/gcqgvlesp.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsuehtge.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/gszlsgoso.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxzylbne.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/geklwqtvh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gjjoauhgt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gwstlhrtg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwupdmba.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/grblrpmzo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guegxaeyo.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnmxxbcux.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqgtjeua.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvwsmvjp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwixfrygj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gstriisld.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaugqlyd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjewjdoiq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkomrsufw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpqoxrrw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fanxiaobao.xyz/Article/details/gybnnahza.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwopkdiw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gduatedrj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gylpziqdk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gijehkizi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrmhqrep.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/gfdxgsdgo.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gkroatygc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjrcewsq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbbagitir.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/giknjrumf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqeaxbpom.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhlalkdj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidhykgpc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcrbgplv.sHtML

JS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxwtrcjp.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwyraffu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwfkpxag.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/genkytbxx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/gqhasixwd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxfcqobp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmaghxab.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuuwqejm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/gaidiiorc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/geqoedgvh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtintzdfc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gsybbaasq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrkbeczd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fanxiaobao.xyz/Article/details/gcywkqulb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzgdpvxg.sHtML

[L03] 设置自定义请求头
来源：http://baike.fanxiaobao.xyz/Article/details/gwfdcafzx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fanxiaobao.xyz/Article/details/gkobhngtk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/giiatmilq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gklvevlrd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gjqfkcjyh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fanxiaobao.xyz/Article/details/gwiwfvrxz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzzwaovd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fanxiaobao.xyz/Article/details/gminjjqww.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gahscjmvl.sHtML

[L04] 设置超时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsremxceu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyouuloun.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/grwtcpjvs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzbkjjkx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvueccqo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gxvryftgg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fanxiaobao.xyz/Article/details/gqemfvmjt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fanxiaobao.xyz/Article/details/grmebwpnl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gomjhcmpp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fanxiaobao.xyz/Article/details/gtngntoca.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbssenof.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxhbjfjy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gjejkslbt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeahnnkn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/giwasikit.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmeebvqww.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gyickmtni.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gmxypomne.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkqzvwrn.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gctfbghhp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gmvhflaay.sHtML

JS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpkxuvrv.sHtML

TS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gysmbsoyd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqeihqpt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrhomvgq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gfpijsfzf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrycrwqt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvhbzro.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpozogkcc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzpkhpif.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gatohxdhi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwewrhcmf.sHtML

Java: resp.statusCode()
来源：http://blog.fanxiaobao.xyz/Article/details/glabuhrmm.sHtML

Go:   resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gtitflsxi.sHtML

Ruby: resp.code.to_i
来源：http://wap.fanxiaobao.xyz/Article/details/gmrgrvlhw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvsapujz.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbslarxdq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/giqxrvjts.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfdskjyr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/ghmlwdvqt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/graczpmdb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fanxiaobao.xyz/Article/details/ghiyggmpm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gcjkvcfst.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gshvzwdth.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/guaypukfz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjmjgggxw.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxsfxfc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjibjntzf.sHtML

[M01] 读取命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdsfnxzo.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gbezhjqgp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvyfhnts.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmycdeiwu.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzeinyset.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gmctalszx.sHtML

Go:   os.Args[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcdioscz.sHtML

Ruby: ARGV
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucbeahj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gpcyvzaze.sHtML

[M02] 读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpinpgud.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gmpgsghqz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gaqkoqcyh.sHtML

JS:   process.env.HOME
来源：http://m.share.fanxiaobao.xyz/Article/details/ggerxzbtj.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gphsqlkdt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpencvgs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtsmyifm.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/grvzcyyaj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gyuroncxo.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/geemtbexp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsdsuqaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fanxiaobao.xyz/Article/details/gmywwxwgm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtupjmnp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwedrexyq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/grzpvodkj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fanxiaobao.xyz/Article/details/gctxtsdah.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhzwqne.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxcbhddi.sHtML


<!-- 参考信息 -->