代发 wailian999

J. 日期与时间
来源：http://blog.fanxiaobao.xyz/Article/details/gvpiqfnue.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyrcklxb.sHtML

[J01] 获取当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gczzwtbtg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzavdsfh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjegoxmnf.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gxwcegonk.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gigcghfyd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gelbgsbsx.sHtML

Go:   time.Now()
来源：http://blog.fanxiaobao.xyz/Article/details/gxgojtygk.sHtML

Ruby: Time.now
来源：http://m.share.fanxiaobao.xyz/Article/details/gudzachxl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fanxiaobao.xyz/Article/details/getkmzrzs.sHtML

[J02] 格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gxodnucmq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gsutwbhez.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdipkzzrv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdevfstz.sHtML

TS:   d.toISOString()
来源：http://blog.fanxiaobao.xyz/Article/details/gybravitt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gkfnffqle.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhqeljzd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzjkoeuv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeczszkj.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqypegnz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gxqeryckk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fanxiaobao.xyz/Article/details/grltmecqf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrqniqcy.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gpzhytocb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gytcokcwp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gapwshung.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagbrzves.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmmiopzy.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxdpcqzd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gzsakdvlq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfzvjpwk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/gbymeuoja.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawafrdrq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxghmzzzg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpmikfdf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrmqcxhj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjdxvvzu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaiximgb.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxnbheyj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/ggblfbjav.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gkgcnzyoi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqhvbue.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gpsvdugnm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gxbrrbicj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqhwhzpw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golcoqsyt.sHtML

[J06] 计算两时间之差
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuuvseul.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwblypax.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkznwqjdu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fanxiaobao.xyz/Article/details/gwzodygvo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fanxiaobao.xyz/Article/details/grojzwhyr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gixspjzew.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgzpojih.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbtvgvco.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoptcehp.sHtML

[J07] 比较两个日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsonympru.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gftvgqwjh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkccgztu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gdjumvfxs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/grvwoiwbt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsdunrjqq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvgbjilc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmsmryem.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gppkxsxuy.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcizgnmy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fanxiaobao.xyz/Article/details/grycxrfqu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmwqprbd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbttphxpx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxjqxmne.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gzxwmauxp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fanxiaobao.xyz/Article/details/gciynkcze.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqvhwqcl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/gbuuuiifr.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqpvnajs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlcwpgtf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fanxiaobao.xyz/Article/details/gotccfbjg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclvpvohg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/ggfznvtuk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/gxpulpbyd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdflaxznc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gttzeamll.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fanxiaobao.xyz/Article/details/geicpfebh.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/gztsorqmf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gksyctsjn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fanxiaobao.xyz/Article/details/gdjbnjsmp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrsrblln.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gxvnosqsc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqidlybwe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fanxiaobao.xyz/Article/details/gdcrvdbnx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqovxnou.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gupfoiuff.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwazoolcl.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/gsvemrpid.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbahiuqgw.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvsrppilo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggevzmcot.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwgdrohd.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxopsgspz.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmrbhjlb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gafamxyws.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gobimlqin.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqcpaxuz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggsqfufeq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fanxiaobao.xyz/Article/details/gmqmmgibm.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gefbciyri.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvaplicr.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsftghkg.sHtML

TS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guxyaqyuk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyttchsfb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gbtdscygv.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjpswpyj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gplrzducc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fanxiaobao.xyz/Article/details/gakkppvbm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmwqbsfd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gtvryywnc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggikvgcbg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvvjhusxr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gugyfxjyg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/guixoapkr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/goapkfnbg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbbxmdsn.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjokkivnb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfmszsbo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gatzhswgg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmccwnzxp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gzoblhhwk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsqmgzii.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxcapbyu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/glfwqpvfq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfgzzwti.sHtML

[K05] 深拷贝对象
来源：http://baike.fanxiaobao.xyz/Article/details/gzinafjtx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/glzlvvbfe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fanxiaobao.xyz/Article/details/gqxopiqjj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcwzzmfc.sHtML

TS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gfigxzfdv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoxzxdce.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fanxiaobao.xyz/Article/details/gccibucyh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gddlujmxg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvkitceu.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fanxiaobao.xyz/Article/details/gedwkiern.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqthlgwd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrdqgjaq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpygveuio.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxelacom.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gctixukpb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvcdyzdb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gizwigqgs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gvszlvqyp.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gihkalrhg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzrusamt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/gswmklwyk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggplgalml.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gjklrysxr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkqtamoj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdogbiekp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gchwbxygc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpqisdmn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/gisehorba.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gkgoljpsu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gclucyrhl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfubgoq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gupzmqbkb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/gqjbkzxzo.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrjbahfm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgrccapj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gnvoitcce.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbmoebujc.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/gwlmpdrki.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqybwfcfp.sHtML

[L01] 发送 GET 请求
来源：http://baike.fanxiaobao.xyz/Article/details/ghkftaohy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gmuohcohu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/ghlngshai.sHtML

JS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjujoybin.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaszjnxfu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fanxiaobao.xyz/Article/details/gudqnsynm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtufnqlw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fanxiaobao.xyz/Article/details/gligkhywz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fanxiaobao.xyz/Article/details/godrmoxsy.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/govubatbj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gluczthju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/gfgwqwroo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greaxqhra.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotcxrqhj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fanxiaobao.xyz/Article/details/gpvanltoz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fanxiaobao.xyz/Article/details/gfvftddzx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcapayog.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmxuxkmi.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjvaijfc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/gbxmfiqjv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdbxwjpsy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqjyumha.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwimwhfn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzdxxkh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gypvtejiy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fanxiaobao.xyz/Article/details/gfrwqgxyj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiygwomx.sHtML

[L04] 设置超时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboosgchx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcxqfeeq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/glgmnigxz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gdabsanzy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gsarzsdrm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlodblib.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfajepyh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gslilncyo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwelfngw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/gjmhbtifc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrspmwne.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnicrstjz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gsixofdih.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjpduwid.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fanxiaobao.xyz/Article/details/gtgfypupj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grsfwarbb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gjyarpfhi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjnzfjly.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gfgscyjje.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmopenwkw.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/grjmquggf.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviwhcwsd.sHtML

TS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzmlgwzz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gdtdbvaso.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzdgxcmx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhjcbxcg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrklrioq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbakpmvhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnbvpmlh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqhkjfzh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/grfmwwszs.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhoqbece.sHtML

Java: resp.statusCode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gztndbbba.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlpsjokb.sHtML

Ruby: resp.code.to_i
来源：http://baike.fanxiaobao.xyz/Article/details/gacwlwxxa.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gpygypskc.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/grnuiasmp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxchftg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwkvboqx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujfmppdn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gaucvxxya.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaqnjujg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/glfaecith.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gigntctnh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gmhgwtghr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guelquzyy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxxaytkv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsflhmqgi.sHtML

[M01] 读取命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmuhpzqj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhbinepw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkujdakxe.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfvlzvqmx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbxuonsg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzharuoa.sHtML

Go:   os.Args[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gazezrzbl.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthcmnhc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gwrszrubv.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gajvfxwmj.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gqcoksvbz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhebcstc.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppsdauvv.sHtML

TS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gzcczwrvk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqgycsqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gikpgjgwf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfofdzpqq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gojcrrwyp.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkmfvqve.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gngmnfafn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzhjumjf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gweuugjyt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsyvyyln.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcipadltl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fanxiaobao.xyz/Article/details/gkiagctpb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruylofpz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/glwolhdmk.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gjpoxcsff.sHtML

Py:   os.getcwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gkbmllgyy.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxvfxyfd.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvixdfrf.sHtML

TS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfgxivpe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fanxiaobao.xyz/Article/details/giojbrgct.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gcjxfkksh.sHtML

Ruby: Dir.pwd
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrlszkxw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexjhorfc.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/greyaofqc.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggrnyrxuv.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrzmvidq.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcyebbauu.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqhaunmvq.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/glpcvroug.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzezfejs.sHtML

Ruby: exit 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutfkkvnf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fanxiaobao.xyz/Article/details/gkbzhzioy.sHtML

[M06] 向标准错误输出
来源：http://3g.fanxiaobao.xyz/Article/details/gbzjtdljn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/goniwryms.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/giuyugyce.sHtML

JS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/glcwpjqql.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmpkxscw.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gcogkqaab.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gdctbbvjl.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/gychbshro.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlafyent.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gvhgbqbpr.sHtML


<!-- 参考信息 -->