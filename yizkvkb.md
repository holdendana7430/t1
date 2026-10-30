代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gmrnrpnhr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gizzcxkal.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gnpjiruyb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjcrozyle.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gaxqyvxba.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gerhplbmf.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ggfubkbqq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gikxuggkt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gzdlgdage.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/ghnoggzco.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gtcyldfjx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gabobilyo.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/ghhebttwm.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/grkeziuuu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gdkprybit.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gdgzfqiuc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gqzjmdgxs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gxmmouehu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gaervvzay.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gcdrnatrt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gwiqhgipo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gpgdvrkls.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gfdbxqipm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gbdbrvmhz.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/glphbdxzp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gktlfqhnb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/geydxbwsj.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/glcjwiwpu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gostuanhc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/govqegoow.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gsibrosua.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gtpkfmqmg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gymvvnhxm.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gkmissqko.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gridptvtc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gzhormodl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvthcsu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gixweftoo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gcxphnmcv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/gjqljmeaa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gemzqhbdx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gikxcypuc.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gzbflpoyv.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gbhafchyi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gnuhnzygz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gkqwrnzfa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/grbsssvzl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gebzmzkoc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gewocqhes.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gcxtkuiln.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gzjwegfks.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gbtctwtzt.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/grmohbgkn.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/guclxengy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/geenkthlz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gerxmhfqy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gktalmamr.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gchldcmni.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/ghxnmiptm.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/ghzhepqfc.sHtML

[J07] 比较两个日期
来源：http://blog.fehbvm.com/Article/details/gtkpngorz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/glmeiaavo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gdexxlvvm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/glhgsyfja.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gossopqra.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/galqdbcvp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/ghsqhiaib.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gxphossoj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gqquibseo.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gannbrcam.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gbllmrkvb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gxuwonhdf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gvhsuxxsi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gvmierize.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gfsxhvnsy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gkwdigrqx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/gimnjzhhu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gzxofsybd.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gayoeuzje.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/ggofeojjs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/globbqbmm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gwqyjvawu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gbiiagvqc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gpnoibnzw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/ghkqrdcqz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gdcddhwqj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gvmtilkge.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gymfwmbzg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/guajegtwi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gftivylrr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnkongjr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gymwglbab.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gphefehmh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gkcrjljyk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/grrrovvbg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gbbodhvur.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkpbbqfvh.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gmtafbgzn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaggsgxmc.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gvkwitjyx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gtrysabuh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gpxvokgbw.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gixruwtgc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/graivhwtr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gvqqosdgn.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyhaterms.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gbyuwpdjd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzfuvsnkw.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gozhbflnx.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gczggvjsc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gtlrawbwb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/grtlceast.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gurxhusxf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gxtuthgrk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gkydwmbin.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gyngfsfeu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gemfodqkx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gnyqjsevb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gpayadrvo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gktkflqoh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gpjcgplhj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gkphufocu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gjnbivsvh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gvvkminxu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/glqpubcjh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gypwvvoxm.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gewsfyzeu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/glplygfvn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gcgzorqxg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gvxbpauuh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gyeqhazed.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gvxmnoazr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/guhzcnvum.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gpzyaubyg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gxrgkbyeh.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gjkxgawcz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggpgrntsb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gvpyppqsp.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gusxrrnei.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gxftefyqv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gzzrpbbvj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gtuugwzmu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gotrzjpoa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gypfbehgd.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gbhftzzrd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gkmszelaq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gljbwpcdq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gctdecyzp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/ghekefezd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gwmelffaq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gegvpwjrh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gsewuirml.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gppzutaho.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gdhhkhech.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/glfgsdsbt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gjatusfct.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gwlhkinla.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gazhrcqjj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfdnxgete.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/galhizzai.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gsxacknkf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/glkrzifqy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gmywgzniy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxqxfxesc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvepiknfg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gzcxakplp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gaqaspros.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/glgyidilx.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gudpcoown.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/guvatxexh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ghhjwtyfp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxrmtwipp.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gcyeumiua.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdrncertp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gwgkqcqah.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgpyrxe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gvgpqgjyv.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gmabreigx.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gabajsodf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/ggnludyvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gcdggpkfh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ggfkdbtci.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gfbelgrra.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gczsmniyy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gisoekbdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gujyevmri.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/guglqarqg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/guyzcinxi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gtcecikwz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gpsidqhhk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gwxdgjbnh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gochwgbtc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gjvkazwpd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gdmdivexa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gttcbzyaz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gsonlzzfq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/ggdfooffg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gyntbrsuz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gamqwrhkw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gzwzsqwxu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/glllkxzek.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gszsqablt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gatpyrxnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gezzxpxmi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gwvxaybsw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gbttgwyfx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gfdgglqml.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gqxtpreon.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gzbwstkcv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/glbxklldd.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/grmsnrgpd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gwqbqkbah.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gmgbcwacp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/grdhzhsxy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ghfqzwdfq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gjaaqfgty.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gajyulmkv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/ggjqstdip.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtzcyfykd.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gtzkdgcza.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gatojcqns.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gxpxbkcbn.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ghtkwrsde.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gvwhkwltt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gvbudsdys.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gafflvheg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvuqmct.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gsuoevcuu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gssuspyfx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gwywhibfm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gjyuygraq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gdkdoaaem.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gyjdkhfkh.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/ghyatckjh.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gpkairhgj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gmfalffsv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gxbydkcpx.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gmqbtigds.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gobhwedcb.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/grpdbxjpx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcvjpsbzb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gitntzlgi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/ghmgvjiaf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gtppeyxqu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/grgxfetli.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gdhttvgid.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glnqwrxxf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/ghmjiuvsf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggruycagk.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gdszrjtyr.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/geoenramj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gckxodcnk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gcxbmvhdx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/ggutarfzj.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gpamcdgjz.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/ggeoitpoz.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gfwznunox.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gimjnurqw.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gvgvkukci.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gvfeucdzi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gsodgyfnh.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gcidkqjrq.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/govjrbiko.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gtrngtqir.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gtphvmkft.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gvwvkafhs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gysuwwdhx.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gkujpypgy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gbciglyfr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/giowyremr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gdecmuagd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gwpobwyub.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/genwjyymr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/ghvbarkzl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gvntcuboj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gprmmerpt.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gcsqvqsvb.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gqcjkbzpt.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gohumnmoz.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/goyafnguz.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gngqlygdy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gmmfkhezz.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/grcfyjsmb.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gdgeqmihj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gygkixhhi.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gtwpvtkso.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/goozgkhgy.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gtamkxdoy.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwmvhiukv.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcnxkeyjn.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/giyenznjh.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gtjuuutkj.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gqxfobskx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gezbgsxrw.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gstxxgbnl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gfxbtmyww.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gfnueaups.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gblqsyyrr.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gtyttuzvs.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gylyhgyia.sHtML


<!-- 参考信息 -->