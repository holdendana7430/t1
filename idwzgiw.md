代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gguloojfo.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gefgxcwmq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gyecyuyus.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gnaavtyku.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gxsuhmwdg.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/ghffgbqdb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/ghiuzyaqz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gvvkcizup.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/ggzibjsxx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gsysuhtmv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/goqmtdfcp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/gojcelvsy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/ghpngcxde.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gfsliarij.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/glqxwiqvr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/grqjukytu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gwvenvusk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gxjieeubc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gphoraxqk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gopgryxto.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gdzrcabnv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsskhdjjw.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/grpompifq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/ghonfpsot.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gukjiimaw.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gphnbxydg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/ghebpipmc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/ghfrhujwg.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gqwzogphu.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gokvfvvkq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gqxlmbmqd.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gmijpwvzx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gpfdbwtkf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gpmpjrqfn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gnofrnzvd.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gqothcdqu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gwkrkvdln.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gftwkofly.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/granbsbxx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fehbvm.com/Article/details/gldriibku.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gmshrsini.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gxykbzuay.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gagdwiysh.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gtjuzfopf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gpjtlokrb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gqrnlggtj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gwmpsnhkg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gkcyaoyct.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gimodjmva.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/geaqvdmbq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gczbqpyew.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gaybvabzq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/ggneutxza.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gbsgydfip.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gygmdxhsm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gujfyrlkg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gyogadohr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gbwxjlobg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/grzfjmcyk.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/gqpkpfqra.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gdocevkzk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gxkxoscqh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvfatex.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gommtvgvr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gbhqdfrsl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gvcllkkpn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/ghbsnlydz.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/ghxreykcp.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gzopguftd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gzujqqkee.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gscfonrmh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gbxdhvncf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.hesvh.cn/Article/details/gezmgspxi.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gmozjtbfv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/graqvagze.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gwgwrsopd.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gukzbldla.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gyecvgxsn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gcizykwuq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gmkzftgju.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gatfqotbj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/geuqzzwwa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/galfewxkh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gypwcrzqu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gixdydyzn.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gwxivzlfw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gmbfaxaqq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gjpfqdvkv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gkqwqieah.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/grvogfbbz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gmovhnvmm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gmhovtadm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gkskbuipp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gcnmhenwd.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gtvwcihpv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gxmxwttde.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/glnnkyirw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gkxrtpxrp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gauadfsgk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gzzgpjxtx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gsowskrrc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gfdtgpmwv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gjyeqcuje.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gjxurgvpd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gebxgbopo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gqznustku.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmvoboeod.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/grjvtoesc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/guwkokoun.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gdfrxtljl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gzkbfrifq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gbvmxsgal.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxhflfays.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gtnkkxvxd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwoyxigvb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfeziqjmp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gxfdhtnph.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gunsfqjyo.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gcasduyqh.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gdqmxfpxc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gsgyedxqm.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/ghienbxkj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gybvscexh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/googlqzfo.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/guzixnnkk.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gasceppkw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gggjwqbue.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gdelpoyrl.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gumehmudh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gxzjkmdkv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gpfkkcoeq.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gbygfvbny.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gvotckysf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gektlpgvy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gnlfvnnjf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gsnxukcwd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gmttkrrbf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gwyrhxnog.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gfzbhqlev.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gvtbjmwul.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gymihpgqx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gsoedbwdp.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gepkyufsr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gochqqbhd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gtmcttvxw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gbebrhtkr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gdiqpalhd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gtokcbkyq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gpygpcxyp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gjyuyixmr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/grxqhndyc.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gywakjmwo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gxpkofuju.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gmuyigdsj.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gapzwmtfc.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gfgwgvgsm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gjtjgynms.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gmzptyrbt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gyxbsgwvb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gllfbpfwp.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gqqnursdn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gdbwulzsq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gkzfwyrjb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gtfohcnrc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gicucepma.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gyxegkxrf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gzgwmwngw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gaboocnnr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gqnwxyhob.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/giysggckc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxzeiwsbj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gldnnhmug.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzfzlkhuf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjynbvxij.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/guchwipqq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gfcubuhbs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gvomfevqo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/guvcyyrdk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/ggvgivoni.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gfeiwoxra.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggzejgzyq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gtiengqci.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gneryxzzx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/guxkrquzp.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gafexqoqr.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gdocdlabs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gfoegumye.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvtouhurk.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/ghrrkyynv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvdfazlld.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/ggqlpijqm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/ghpwojsog.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gvcwhkjik.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gwmmgaxgi.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gtgmcdtxh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/glwdghpbd.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gakxuusvx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/ghtbtkgoo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gptlrocsa.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gcmirkcsd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/guisfvdrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gbtncpxby.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gtlhcfqca.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gnhmeuvvq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gspqzijaz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/grwtijyjx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gwozuckpa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gkliavfea.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gjewjylms.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/guipegwln.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gszowebjl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gmubdduth.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gdwokinst.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/grwrowjhq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/grtqcfnsq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gulhunsiz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gudiewfeq.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/guwqdttok.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gvxjzwsry.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gmjtuxjyt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gprhvubiy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gmoljnnnw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gajdejnol.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gpcidphbo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gosjczkbc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/glmqndedv.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/grcbztdbi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/ggzpfliwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/guuezpxbd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gmlgwrwyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gtqdalyec.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gjxaejjpt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gqsvrsdkd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gibjiurjp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/glxyfoipf.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gphbczeev.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gaqnlxoej.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gnewuzbwq.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gsyoagtdc.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gxpneopbn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/glazzwkbm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gddrmbhle.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gknbnatqp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gnraagazm.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gaaqvnwne.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gjmtrcccy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gwndfhfzu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gqnwgjwau.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gkjeetgrx.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gmsfozyya.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gcdzaxmmx.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gonhcvimh.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gfrxsmfba.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gfoyebboj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/glhjmabka.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gazsntwkr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/glslivele.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpnfwdwnj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gefnjzynr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gwrdmzekk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gmnessltf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gyzyshdst.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxoewnezz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gzlunpzlj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyuarbsha.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gywssvlrs.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gstmqiaks.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gbnwklmvg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gjfyggscp.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gagencgwj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gxrialqmg.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gwixvfocv.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gmjbkbnmt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwoaktlsl.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gbomxxgkm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glrnmirex.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/glqakkkiz.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ghfdmuehj.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gwpjmnqqh.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gytftghlm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gfdxytttf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gcapgxojz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbkdzkrew.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gxkqwkdmn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gokjpaqig.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gohcftekh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gbxtpdkzw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gwniwxybj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gobsgwmnw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gutgbbfni.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/ghqvrjwcf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gjyrhglcc.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gxotzznoh.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/geylfkojb.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gjqxkfouv.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwirojjgf.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gblwhkvil.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gdjzoaduv.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/ghqoawcjp.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/glhsntdip.sHtML


<!-- 参考信息 -->