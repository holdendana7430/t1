代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gamdeuyze.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gzwtkxydo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/giypqcyck.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnkbafaam.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gtzoawjlr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/getgejopm.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gmhfsklwn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gzpjndcrr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gefwqxcgb.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gvbhbihbj.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/ghucagvsj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/grqlupczi.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gpxxsrcsc.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gyeffaepv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gcrozrnsu.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gescohhxj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gqstxzsqk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gwylvskde.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gntclqypu.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/ggjerqkky.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gihmhjtsf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/gepokhcye.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmpbgogo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/garteorcp.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gzscslgno.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/glguvmrus.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/grkjafwck.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gvgvlimzs.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gnzqjarhv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gxsgteztl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/guvlpmtzl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ghzryvift.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gskrtambv.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gnimctlrw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gpmvqdlwi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gmcaalsir.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/gthpxhbfs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gaxilddif.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gndaeqbzi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gqyzrugqh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/gxdjfmrwb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/gdhtnbmmq.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gdfigvmyf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gduqljphs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gfpgmhjdr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gqintdiwo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gqfijfehu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gvcdxvvmp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/ghddlborg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gtyvgwxqy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gbgbtiowj.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gxbklyvvu.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gvjaugzlz.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gkpbgpypq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/grrnmdnho.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/ggtpsknca.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gpsztckke.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gimcrsodw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/guxvwrnqs.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gdayzvogk.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gvhqfwcbs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gxqlvhxvg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gjmcwpnjt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/grijayxkr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/geappouil.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/ghvecypyj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gcymdtwfg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/ghxfafnwo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gbcorgobj.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gqpxmybfd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gmqrwmeuc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gusenoqiy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gmqtkacka.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gbcilpsjw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gbkegkbjw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gyolkxrur.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gtlfzbcth.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gaeklizqf.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gnszupnlq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gpnyaobbc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/grmlvgsdq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/ghtgwxesm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gufikrhcd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gfruffumb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gdcdenjhx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gutsscxpo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/grtpvipdv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gknkdusls.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gvrolxrlb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gifmhmvcj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggajhhygq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gclwbhrfl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gqawvccwc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gzecaxkyw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gagrqqybe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gzfpfwsxs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gexurzjly.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/goaatvdpy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/galuafysm.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gbtrxyzov.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/ghvcppsyc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gzrdxegfc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gctdhvruj.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gkboaypmn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gryfvqvsy.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gnzpdyqyt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gqpydiilr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gwjovooqj.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/glrtcufca.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gazcbuwsn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjscelbki.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ghkbxznwy.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gwbehxxpq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gkyvcpkmo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/ghpnesuqw.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gruajxvya.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/goofwuprt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gkbitdbtl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gxlrbknlv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gkkezytmq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gmpwmkwdp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gsddotobq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gonfbrsqc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gqgqpfgzn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gwvfalzao.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gwylbbhie.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gouqxpiez.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gwbiilccg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gnfrkhiml.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gucthbmql.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gxgaahycg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gojgyykcm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/ggdpqgxdh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/geghvpwav.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gbiulsvwm.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gqlvwxxqr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/guvidaqqc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gigfktqrq.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxzpnocag.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gvemtonni.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gcbfomrfl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/grlyrnvpu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gomxfrueb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gmaoswgsw.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gswitiozj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gpamyeskn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/ghelxzmum.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gkkdtvnpq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/glurtdhbh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gcwhxbgpb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gqkalueuv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gekawzugd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/ghwlynyvo.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gxaphuzzi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvrfegkis.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gonbyxzea.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gokyvjpfx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkeprcy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/grbaxoppt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gwhwwfyap.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gtogpbnsr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gdbsdvwro.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gbkqtrkkh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbcsqgdcd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gtstxpwha.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gnsurjxji.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gfagenaut.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gjwyvwhyf.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gcccrbacx.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/guavhjhvn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gtwuxwodz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzfknkp.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gnxsxijey.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkdcsmhdp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gcipqdnnd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/ghtycexqe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gsogqrkdk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/glfdmjfyp.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gaorjwikp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gxilbymzy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/glpsnxzct.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gysfcaywd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/getmtpaxi.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gaguheqpd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gnherykbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/guihbfvdp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/ghgqamozh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gsrsmnqwq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gezgrltwi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gyiqgakpm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gqhnqcjcp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gbvyjjmel.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gmghdpyvp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gnirnrhau.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gopkriyrf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjhxwwg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/guhjkuqdu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/guuqpemwu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gqimllnzm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gfwunuaqq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gcfkghnpi.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gzyvdsbwr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/givaxsuym.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gdmvmypkq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gljqwkfos.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gimtqnggn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/ghnfwyfgi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gsckiiwvn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/guqvkidou.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gcytmndqh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gjgxeasgy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gwkwxqkjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gmcrmstlt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gnkzmwjaj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/grlqlxgjy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gjsdvuvhn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gcunvctqy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gpwotqfju.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/grwlntxkr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gcicqqosg.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/glzjgsyal.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpxuufgwi.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gozuwccep.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gfwfkauke.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gqbrcwoeo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnnkbwvf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gbsptscxd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gvdecxdah.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/glyexqogy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gylytsqwd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gcyobpgxs.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gjtqffujf.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gtmyuwvmb.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gdfytodiv.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gkctdndws.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gigwgjplj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gjuxswmsc.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/garrsnlmj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/ginexurrh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gulphlmix.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gqgzdiiwd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/grukxxerq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gunuivwdk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gfpcmrqgg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gdatdpdny.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gmwvtdcge.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaedoueiy.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gbuldedcp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwpbzeszf.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gsuzfauag.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gpqmuwyhb.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/ghxyajdnx.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmqmeskoc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gvsfzidda.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gepnflvyu.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/ghieyrfez.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gczeqflhn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ghdtshzmt.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gaegrhtbp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gexxxjtpt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gdhmxpnts.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gipchlbfb.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ggmffvzlz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gfcbgpzzo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gmwbdkxbs.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gahkzcdxw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/goucdhpvr.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gxwojymun.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gbcdyzngb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gsonyuxcp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gwtmzkdrk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gjzlfrett.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gjtqsjfwr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gbiqvuodt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gzywfomfs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/geqqawqat.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gmejmqgbv.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/ggvuacfnf.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gnieqhhgn.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gwkxgwkvu.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gvcmwddyi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gvnypbsdf.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gdroobdba.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gvgsqhcnw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gfpispguy.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/ghqilnhix.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gofiioxll.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gvuejrgom.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsluepayx.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gaybalbxi.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glblrezbx.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gugdsyilu.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gqfqfdlfz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/ghoyntgsl.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gfujcajae.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/geutgjbzu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gcscsabcu.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gpqzgkqoi.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gfycjsecp.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggcyopbgc.sHtML


<!-- 参考信息 -->