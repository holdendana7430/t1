代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gafvkknoz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gglsaymjp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gvibkloda.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gckhtkkxw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gwmrmrrla.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gjystuany.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/grzkugfnk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gehpuuqkk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gnvnrtnaj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gzdzvgfcj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gbahehcag.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gyiiaqdll.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gikdcqnfv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gvpphuask.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gsnvdmcsg.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gmtqvjvxh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gcbzgzxuw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/guqmitvmb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gtxznzplc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gpfvomwiy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gzyvevoga.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gvtufrxya.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gufrzvbvf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/guadtqfvh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gvodelsmx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gssfgtrmo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gkciphnlx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gzuzcuzhy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gjcrwgxlw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/glkbmlroy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gkkfqyuax.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gcqzmnham.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gciblhhsu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gweqnvhlt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gcmlmahpq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gbldlqzck.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gmdcctllf.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gzbgajely.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gdkohndku.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gruftddna.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gfqrccizn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/ggnknjpxm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gwdgdwrrv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gpghmxgda.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/grisqfftt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gnwxgqjqp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gvlwyqafk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gegcguhif.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.hesvh.cn/Article/details/gvtvslpxg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gumfiyect.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gsqzodnba.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gygogpcfw.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gbspmrven.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmuphwblj.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gngkfgsan.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gbzxkbrrc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/goyzonfbe.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gmtfmxdcs.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gxxoiutxr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gzkrngprp.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gorljxxvc.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gebtqwdeo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/glbnzfoig.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gbudiyvsl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gboepigat.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/ghesvwuue.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gqyrpduqu.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gqlruulvp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gkglfnkje.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gdyjxirst.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/godfmcuna.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gnkevubhq.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gthrhisld.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/grohooegk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/giwkqtjko.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gcabbjzlf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/giaijvcmg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/ggyfwywus.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gcufojvgt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gpymbidon.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gfdovjdvq.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/ghzfqkclq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/glvmwsqzl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/glabjfixg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gddnteiaz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/goblnbvcr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gormmisat.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gpqoujjdy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gjdoqtegj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gmyncxyiq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/guxdkfihu.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gzqetfszd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/geuybyfkx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gswmbfcic.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gqpvgbbqj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gfntaymku.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gzgepthdz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gyixhhcch.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gyvnzmdvi.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/geaelblud.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/glsubqbra.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/ghttkemfl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/glmcpdcvo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gpouhmdvz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gmcuwhjdd.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gqbooldec.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gdetejtph.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gtgzqkogv.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/gdojnzssa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gqzunqbds.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gjpiyplmu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/ghjuurknw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gkumihxab.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gkjveedyt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gbhvimkbp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/glbzvupzf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gthzvtutc.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gaaanxzoy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gfsaawtwm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gqqitscdz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/gxyvsrrrn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gwepcpdvz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gionvujnd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gzlznmtoa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gvozabbuf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/ggeegbegm.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gfkigorfn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gdyariely.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gorbmelwf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gxaloopvj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gakytqxkv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gvrxdubus.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gzvgsxsrt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gwxwuawdq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gpzqohqdq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gcqxlnfpm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gwcajkgry.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gqgwzqhgx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gpteznxdr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gzpyggaqq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcbjrmyo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gdifuzgbs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/ggezniwna.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/grevndkqj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goksexvgo.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gitzlqezs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gymbyandq.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gflgorwvs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gebjawanb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gbuqugcvf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gnpbavxyd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfdtaglpo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gmhmgrmmn.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/ghlhvuhez.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/goavausjm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gyhwlleng.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gyhpcrzsl.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gjabhvsga.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gqptkmhht.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gkvzhuyso.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gzrzjezvq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gbieipvof.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gommrjufw.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gnsfzeenx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/glqmzrnxh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/goesqfsaq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gleztuabr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gjqvfvsfu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gigothuuh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjlqsabzl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkuadtrwp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gvfdpltsf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gbnntothr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/ggrrrvtxb.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gbrzffgxy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/givekbqrk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/geitdixki.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gqqnsazxk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gwfywdooc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/glfkjlegc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gpaoicwns.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/ggcotdzgk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/guuehoucm.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gnmqwfpid.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gfjnrfrhb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gahthbowp.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gpeupfzsg.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvpqbyovs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/ggtfikhdy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gngorigle.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gxliboreh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/glwusstqm.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gwexxaosc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gzdrsbops.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gsnxeebsz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/giozdrxmx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gcredgjgr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/ghgnceqba.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gjzqhynuq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/glccwylqd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gurompyba.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gxekcnkil.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gflcddojr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/ggtovizrk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbcvvxyiw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxvapdfyc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ghpxungnr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gbmdvxpor.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gdyfdakvl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gkyrfcluy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gwgdjissa.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/goynjifvj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxjbjloeh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/goarynycf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gbrbkaiix.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gqldsjqul.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gmgbywodr.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gupqlelgn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbvbbsgwx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcqaauvja.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gsluslnjc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghfmdzrhc.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gusqjipyv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gardoweeh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gyzpdlvsq.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gipwwvnmz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gynwpmmar.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gbyfaeahe.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gvpjpfaol.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gmagbbfes.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gxmonvepi.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gaxcugiwk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/giqntzsgz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gzgtvkafb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gxuokceup.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/glminbszc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gpykwbgtk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gnykikksv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gjkpruoom.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gjwaseleu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/ghzmifina.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gnqvijicy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/grtnzdzoi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gfogqpkec.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gfusploon.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gdcvrkhik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gxqqjwtls.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gkjfhkqma.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gdmsarqco.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gmrcwjyze.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gycotfalo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/ggykecieh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gwleeousx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gfdbfvhdy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gurwrwgdj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gmebmjawi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gohdlgvyn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gvjrcuwae.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gydflbvke.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gfwcieecq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gfciacnvl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gzkoqsucy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gknjznwqf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gwmmnmrli.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gwnojqqfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gmqbzgopl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggnhqvfyc.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/ghzeypkzr.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gwqcgzhtx.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gpgzrxehd.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gzqptivla.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/glifslekn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gutpurmpm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gmqhkmkgi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gkffytqzm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/grthwqxwa.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gknegclvc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gryyjyvcb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gczbgziix.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/grvbbgbdg.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gmefonjwo.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gdsljbrpe.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/ghogcwzyq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gttljpbss.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gxmkhcfrw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gtzfilvti.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gmplbgaem.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/ghrphodgf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gioujuzwc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/goauokidi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gwkqagawo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gjmptixob.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/ggdorjodj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/ghoykaffi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gadqolmmj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gtmmobvuh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gisnwosbk.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/grherolvy.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gjgtbjxxy.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gisxiitrr.sHtML


<!-- 参考信息 -->