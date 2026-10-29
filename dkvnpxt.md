代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/ghlpadpvg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gprrtbdae.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/ghkgessnu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyhslqkqp.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/grvjhmbnz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtlafmsmi.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ggadswmwp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gqtwqlozo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gdrxrgohx.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gcefhgimt.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gmqhwrxmb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gxkthqnge.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gqyozgllc.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gahwhryea.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gneiwsxat.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gbsvhgkvk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gkwmcidza.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gkomfnkgb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gfpjtvjny.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gtdfcwnkk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/garlwwraa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gxqtgechy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gdwqmvout.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fehbvm.com/Article/details/gjeslizrd.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/goueeeqrq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gvvxvgwnu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gkpleekms.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gevcizjvc.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gjwxtjubt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gznfcppcf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gawytekvd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gokjuktrc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/glnqgakal.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gauipqjej.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gslotpequ.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gjtjuojvr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gbdxwyubv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/gfraoymhi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/gmfgykmci.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzfrzubvy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gkjijlvep.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gmkjfbfet.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gxvvmxpnk.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gwokffqdg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/grnyzmmnr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/guwucgimi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gtiepomnd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gvudnndcc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.zdbjq.cn/Article/details/gavuyehnk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gdgvcbdmt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/geielzsnn.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/guswytptv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gomnupncr.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gdjrezdmq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gcllbskkq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gaxrshmob.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gozivbugs.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gyygyflht.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gwryejqeq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gxqqhadml.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/giwjxvxmo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gfxiojpmi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gcrpexywt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gdqpzjaue.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gvpusower.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/ggzmioiwp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gcjudtcig.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gievvpjmg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gbwvfjext.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/ghlntvlea.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/glibtbcev.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gziiwimdj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gpykvhvst.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gwngehtyx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gtqtahnho.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gvsrzfxcu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gtzljxkut.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gzaimrtwo.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gjcgquezu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/godkhjydu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gfkeijsok.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gngxynabm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gmtvmimfk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gbhztoviy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gtwczczam.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/grodudrjo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gpwcdnbdj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gqkytjmpg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/ggxvatsfi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/guwohzwmn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gaadetorf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdapkoshq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gcwbsglnf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gkfbiovlc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gbyrxjlwo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gngtbgffw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdtahmluw.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/giryaadrw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjkoixwsf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/goawcozio.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/glbkouinv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gkavghfqm.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gahtoehqx.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gxynqeyye.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gjzebsztm.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gxrnuidsx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gdfmceuba.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwjswbssu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gqjtiauni.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gvoevsdrm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gaivljcuv.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gmbcobbin.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gwfswvwtr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcnipwkq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gsfjafgzx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gyjnjecrq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gygmdilws.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gufpupzyq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gyqjnkqbg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gcudgpanx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gqvmkfbay.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gfabvdwdl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzndsucya.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gvqdbknsw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gmgwqbvqn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gshrfpmyo.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/grnziuyxn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/geylwvbyt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gkccccqjl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gxtyurwsx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gdtgnlghc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gvkzlxaox.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gmvjedjie.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/ggsvlysvy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/glhfwcnke.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gugiiushl.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gffyqatgg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gvomlwnkb.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gomtjhvmu.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gogosqrkg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gexwdnkjd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gbbamztih.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gxslkbugb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gflwhakpb.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gfvsuewxc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/giddqqfne.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gkynwacdn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gtzeahtmq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gchudcbmg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/ggqtuapez.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gpbdbwbvy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gqbsaruby.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gdquonpqz.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/ggwzhaxug.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/guptbcdlm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/ghlghssna.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gnmefbeey.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gwnsoylty.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggiwlxkkw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gydfvqchs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gvtjujrqt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gqjlbgtur.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gpbrkxeem.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gggksctnh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gibhmyagu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gzjjfadio.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/giiqflrhn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gvsbfphaw.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/ggjwpriyf.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gbxvwglts.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ghcjccydw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvtamrjbd.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gxzdpofvi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpykhyvfv.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gzfmxauax.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gysxvcodl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gcilsflmv.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/grjtvgwdq.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gamouwmfr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gbapgefhh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/ghlfucnqq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/grbdpxmmz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnfydnohm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/govanorxc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gkmcegfah.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gbwqilmjf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gxpbgiwvo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/geuscmdiy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gbbsntwva.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/ggjoaomhw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gwxdnaotw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gnvcmoqxo.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gzkobvxao.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvigqng.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/ggrnxnvvu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gigwhgoxj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gdznwlsua.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/giueafzrd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gcsxhjavp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gtaufczjy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gpfoiuhhm.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gjbujsnmw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gtjztoxdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gtezwpdae.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/grlqvbkyy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gqcafcmro.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gpzzrufhp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gblodzpcb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gruaydpoi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gcjszztxi.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/geaojmcah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gvbsqoolj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gprejlweb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gbelofqvs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gtkxeyscn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gpuysokja.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gvzfmvani.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gcuiidtgl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gezmsxpki.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gdcgnffqa.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gmlhgijaf.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gahozkneo.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gcajmyqfs.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gibayvwik.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsdpdffls.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gdahwakql.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/goczgaykb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gzvdknuqn.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gxksgbvfn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gpqlnxify.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gsdkzusvx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/ggufqervd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gwmhzjttr.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gsccmfilq.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gjkjkwzpi.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gtdyqmzny.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/glhsmiuyi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/ghlyextke.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gdokvcuml.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/glqyimvei.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ggbloiptv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkfgxscdj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gdkiahegw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gtzoqntot.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gspfemlni.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gkraerkqb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmpjydaox.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gagmubkkn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilkltypq.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpuonexze.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gagoyfvkj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gfxfntkre.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gwdkmgcgc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/glvyasajf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gznqczstv.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/ghmxgaehr.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gcetuthip.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ghcsdcybs.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/goxalilwr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gavbdgbuv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gmhsgjxlv.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gugbhgmtv.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gspkhngxh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtlapzbej.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gnkkklkyq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gtiwmpwic.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gcqddiark.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gkosmrgob.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gwmkesgaq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gtpbvohom.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gszbldcvm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gwwdtqpsf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gyeujazkk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/grimtgigl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gsmocuyuf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gpoecvpis.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gzdxdoyxz.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/ghzujduaq.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gtofnatrx.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gndjmxznt.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/ghmzhbria.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gpthcsdua.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gfiavviux.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gavxkzmnx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gfnkbapts.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gdfkkemqr.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxazkdqlc.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gtxqdxjar.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsnomklfe.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/glvfafhhq.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpfeiztlo.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gpqlnpcxx.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gjbmotzls.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gxzifmlsw.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gnzcidmxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gtwqsryis.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gcbedcwkq.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gkmpwcwcf.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gcklzjebg.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gvgzmghpp.sHtML


<!-- 参考信息 -->