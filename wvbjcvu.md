代发 wailian999

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gukutndhn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gofothcyn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gihloxgny.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gipyjvhqk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gqinrfses.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gfgpjrvdc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gwdpsjmoi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gbqnagnhv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gswxhuwhd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gotdszqqm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gbkuuwkbf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvurbpxbe.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gvzenzgdw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdpqnbkde.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/glvfvrzxs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gguejxwiq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gwpvwmjbd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gfqkgbnxg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gjfpuzdlh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gawyrrxqq.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gafgrhcmu.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gpqlpmkid.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gkdqcffmd.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gdxvmdbso.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gymeokjmz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gmaubmmbc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gbwpfusqf.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gdbjgslet.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/grmxqkrch.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gnhccxvmo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gggobwvdd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gjmmjygtf.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/ghqlnqevf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gmctnzkzd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gzyjcuddi.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gulfpcavs.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gqzhkhvno.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/giqaxhdhz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gvojlqdlj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gtpnhtlux.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gmjhyhmfi.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gmjodlukk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gorjpztul.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/goipqofoe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gajkgrhtb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gajrqezcq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gqaqzjeia.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/grrbwjmfs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gguqyglch.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gtdqynjtu.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gcmjtcyzi.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gkeytpjxj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gserxwqox.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gjlogqdhm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gxzfmykbt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/ggccbkegp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gckxrcuvl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gairvdiyn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gxowzkdik.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gzulwmcuy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gxrfiaoit.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gwqvukwio.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/goodqnbnb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gsneuvfyz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gljkdmzxf.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gbhsxbvga.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gwfgagimd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gdhjihinf.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gvjqbflao.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gqdmszosa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gnlhnlibp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gguvzckrx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gqcmbunix.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gfkiwmlze.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gmgmepzqb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gegzxwhzm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gbeaxcyxr.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/galfrjpko.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gwdzwqige.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gfaqnaxxv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/goqlpgvkn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gysuelzzx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gcqkjyfvb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/geigikrvd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gdblwifwg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gppmnsvrb.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/goaiiidly.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gsxsqtdij.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/ghntyodax.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gwhrjsjgf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/grdcefdba.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gnchngfou.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gpxsqkbpz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gihmlvjxz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gydkvhkph.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gompqbmfs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gwvcacpdn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gwaxkciff.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqviiqzcj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/ghtjkbmri.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/goimwoiiy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gjcwpoywk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gdymeeyhe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/gfdstmzqa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmbnqbsmk.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/geycmltne.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqfqbzefw.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gcoxbqbfm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gjsprwpxz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gnsjhxinl.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gmqcmdwcw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grmydewko.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gexoisgxk.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfgtxwmaz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gyxpjdvpz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gsknsnvyj.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gpbadfzmj.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/ghoryxxkq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gctkaaces.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gkreduzkr.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gzvnlffnb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gwrpezjbf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ghennetny.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gzvqftsgd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/grsxviftz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gpcmswrzq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gtvexarri.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gycnzcuxj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gpzezbpbg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gvyfrzghd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gogkhmaww.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gtvqmudmy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gskuybxpb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gzcpgkpbm.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gawcyabss.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gyqxiwqdt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gydgsmuah.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gjhmzsjuw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gkaaapcfx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gouasrzfr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/ghdygsiyy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/ggthlhdgo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gkrvdbftq.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gborzghvl.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gbrkxtgtx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gtyhnhxgc.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdubbwkoj.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gvpxojekt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/grbpvfqrz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gebyqwnnz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gddlrjjqb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gakcuasay.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/giplzhaft.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gfiwgtbyf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gbtbztoph.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gbrpzhhjm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gszinnwdc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gvcynbxrq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gzhedwnjr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/grlqskxsz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gfueukivl.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gmxsejhuh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gbwowwdto.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gimbmlanz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gcoylsyun.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gliyrxkqa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/garwdwcoc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/guqupceys.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gfxrnofig.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcreytglb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gcecazqfp.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gzzdfsctt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/genzsgsco.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gtumwwjyx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/grxyzrjxk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gsuashgly.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gqjpzdoos.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/ggpwgmlmr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gtrtgwlut.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmzgzyoir.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gqriommaf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gflplguij.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gzqiqurdf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/ggyjntrdl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gcichxuim.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gvmzndhmx.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gzxitdtak.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gwxtugocl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gihonyuxb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gmmglvjdn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gsajpqsqq.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gyydcsofd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gmheohggw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gklewqhpm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gpaoiqtkm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/grgkfamah.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gmfczrapg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gcbuvamru.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gerzoukxs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/ghzmuclyt.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gqbhgbhih.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gyepzfgqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gmeeoorhg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gzeveqqzx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhbaspb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gcsosqatz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gllkfxccd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gldfsktnu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gftfcoxli.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gldeljodn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gyjxutish.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gryhkvryr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/geuhxoxdj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gfeihmqka.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/geexosjps.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/guyymwfof.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/guoygbcgk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gfctvkrij.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gmiloryzn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/ggrsdtfbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gujvgearj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gjxmztiyf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gbkhmicpb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gzrpkqtwr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gllhzjzwc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gaigjvyae.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/ghaxsuxzs.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gmzkdfeuz.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gwdhqoakm.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/guvyvesjy.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gwlznifdx.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gstkebknu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gfmmwosgu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gwmaxdekj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfmgibzt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gecepchah.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/glaubjvon.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/golcoisvh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/glznaogng.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gsynrroke.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gfsptbplj.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gjckqdhqp.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gzrxdlcyc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gsaipfegn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gsvsffbcs.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gyvrsmmjb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gjygpstmm.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gsjsjfsta.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gudliysix.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gtjfoefyv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gcvwionbi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gjrfxvvzp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gxolqhkfa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gffdgsitg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfkhbmjsu.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gvzaeprww.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gevuujlad.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gnsjuwykr.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnrimejil.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gxpdtbteq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gwvooucne.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gmtjhrwzk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gaccdzhpj.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/grjskoati.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gklzfuikh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gqstxgslp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gjzepryno.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gtwntkoal.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gemopsvjp.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grjtujrus.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gjatgapss.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gvhvqwlqx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gugqwmkce.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gddwknmxq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gguiqvqgc.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gfovlonkj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gkxfsadzw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/geawcmbmt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/girtztdrl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/giqaeyhqg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gninzwprn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gaveeitaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gkbgqycjh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnvkvbt.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gjbwfgwzu.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggsvucpsc.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/ganujmleu.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gwfmofbbq.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gsvumosrm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/goxafdwze.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gxsbrojge.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gaxtehqro.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gfsusvvrx.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gbsmwvywy.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggzjssyrb.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gbarpkwpg.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnkrxbabv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grzqlelwv.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/ggrmfbfjc.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsyaqzqrv.sHtML


<!-- 参考信息 -->