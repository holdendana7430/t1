代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gkyqzpfio.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdkqmbbcj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gplcesctb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/glkidxhgg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gsuxqwlru.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gmhtplcyd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/genynwdij.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gtbbnhzif.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gyosycwov.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gywjbtklc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gakulovay.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gwxlijees.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gaihskopf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gaoizbjyl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gxqqpnrag.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gyyavblhb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gsaydyohf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gcshbalfx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/getsepscz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gtfhpclpc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/grprgrowy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gnjlsbupi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gqzrjdzpq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gzdfmmogo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gatupvqow.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gopscmzsv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gfkxotjwi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gnoghlmkt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gzvlaldjq.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gabucraxf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gpcqvufjo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gpagwsxig.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gnqxpsdxo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/groptvmvp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/grdidwneq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/ggvgeiqzo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/ggzfugvke.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/goexdjkky.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gobkuhmme.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gpzikixux.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/grupiaabb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gihyvxwng.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gmtvowxvf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gohzoyznv.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gavgwubjh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghptucpes.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gxqgmwocf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gtrfmlygc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gzqccyilf.sHtML

JS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gvcislqrh.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gvtryntok.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gwscexxcf.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gnyyqdzpa.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/gczepyxno.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gxfkqxgds.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gpjsuxoau.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gkvtqggcf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/ghuybkueh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gpzgzqizs.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gfyjxwfir.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gajzxarfi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gnndlgvxx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gurkoinvs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gtudhqtbm.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gmqszyext.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gnvbydkcz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gwkqsaizy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/grhlmaiwp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gpokwppbd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/guaajbgnx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gsafzqsct.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gpquvvsyd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gsowwxhyk.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gktlaphtu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/guyrniyxh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gbloecqxn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gesetewhd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gsjepdjfj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/ggzsucgzk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbevusrvf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gsgjxbwgu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gtdoxrjvj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqxehry.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gmgyizoye.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gejpxfweq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gfzngljyk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gocvxxmqw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gqtwocuto.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/gexvcgyax.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gwgepszbo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/govbulfdn.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gsknnmbky.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gffaavupi.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gowohmavl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gjudpsrkz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gczgutkmi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gmgegnefc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gsmsswuyt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gtcujiidy.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/ghigffmdp.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gpmfitzms.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gjfcvsnac.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/giypwnoup.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gyrnozvhq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/ghtmbxwdx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gwzkiassm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.zdbjq.cn/Article/details/gqmsgthvp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gekhldtfd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gqvgiwqxr.sHtML

[J08] 提取年月日与星期
来源：http://mobile.hesvh.cn/Article/details/ghzvrexor.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gkkcxhtzo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/ggvawodru.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/guqoirycc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gmhdxcqwa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqobipg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gophrjdkl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gyvlijqgj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gdwnhcnux.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/ghsymppqy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gdnjzfqqx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gjlhmxgbu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gcurzuzct.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gbelrhuje.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/goykzdwiw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gzcegkjds.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gdcetsnyu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gqqgptudq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/grsrkomfk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gfzbutoaa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gqprjysaw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/grjickhta.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gopfsmdjj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gzjnciose.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gseydsnds.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gbvnxojga.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwskhmmsk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/govptnhtp.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/ghujiwgzf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/golpryerm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gqhkgbfmx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gewbkagfn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gvrxzftdh.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gyjnuphux.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gaicgimck.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gzivdcyzt.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gcphlwugo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gclulnhtn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/giafnusrc.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gxrbztwud.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gqxgnpgsw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gijdliead.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcclfjraq.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gxxdqwsjp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/godxvdiyz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gcinfsmrq.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gwocmxvpy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gkegjrzgb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gacogkomr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gynpzurqo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gawdbbcgb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gityvuuhx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gveluaecz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/giminycov.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gddcvgvqn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gxdcioujc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gycjvnhfw.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gtvthxliw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gkfhqcwua.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gadjixglu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gumfliisp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gruxyeihp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gqewbxuit.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gqdeygpfp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gkurvuvrk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/guxlafmnk.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gphqgdprk.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gunfdrqhy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gmbypuzya.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gqiicblcr.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/guldsogrp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gfyqczmvq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gbtnxeaxd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gtiisiehi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/grvrxcmac.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gfypersal.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/guvlfgvof.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gptjgllsf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gmadaaxmv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gblfftmir.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gzhlmkoye.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/glxuczkex.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gyhupqaoy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/ggypzhavm.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gqewsizib.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcanwimcc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gpyuqdxyy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ghxggdcjn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gaqmjihhj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gmqnpprou.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/getztdqzx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gfpsgkvhc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/garvbuwbc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/ghcymexvi.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gndximdto.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwkkwnail.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gqzlqojio.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gzgtbhzts.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gwserxvfj.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gyqwuogyb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfdxahhjg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gtoacxkfi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjfrclyoy.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gqsdgjaqn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqftbxqgm.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gqapsvben.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gnxshevmr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gxxzonrhd.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gcobhyaoq.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfvegfzjh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gkzzhqsab.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gclrdnvft.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gsimnokda.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gocfgtuvr.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gmqtssihu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gxrruyzyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/glbwufqqo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/ggpewprni.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gjagnucrz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gzcrrwodg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gbnrtaggx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gzqvpnxxi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gieskwxrp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gavbbrbem.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/ggrzeiegz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gesupkylu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gkmkjkhib.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gyendjsvm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/geexcxtao.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gpbvtnxux.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gkpepjfyu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/glfnskaze.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gcorisswb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gpinuboss.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/giwkcxlfo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gzebkciqz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/grpcjlzld.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gfbyxnsib.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gtmbvtpvh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gdlnaumnx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gkbawbrdz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/ghllgeutd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gfoiotjpd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gjscfkzwk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/guqevgxqv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/glccfdfbm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gimcdgznu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/grdzpvqnf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gaeykumli.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzudmabnb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/geebaejak.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gyxwmzhys.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/grjorllbb.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gnvgcrpby.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gqtjdibni.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/ggaclthkk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gpiojwugl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/galxqlzjd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gvbsdjmyb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gvklxbsgg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/ghozpumnk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gqsbtpddn.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/grzjqiqhu.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gjyqujxly.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gutpnvqad.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gjahclckw.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gcibbmxfk.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gtnqgxssk.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gvwqihqcr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/guwwhzlnp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/grkyxmswt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gzevxwuuj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/ggyhkzvci.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gtroewrnj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gyczxwreu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gjtajidmw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gexmianlm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grgyaxcit.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gncgmkipv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gphmvyvlt.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gvpqodvbj.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gibroexfm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gezwcvdka.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/giivsamqo.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gcoyzsxvp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gxofwmiox.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gvbrjbbow.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gmoywjpws.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gytzyigvg.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gjipicjmd.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gegqhptpw.sHtML


<!-- 参考信息 -->