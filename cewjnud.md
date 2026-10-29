代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gqioiwikf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gdckudewq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/grkhkthxz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gabddibpi.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gnfrcoutg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvxnlcjbn.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gimspbnfi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/gezivkkmy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gohpgeqxz.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gnrxxdpvu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/ggwalezyk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.zdbjq.cn/Article/details/gucicdjsp.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gdhzogumo.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gtgluqsrb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gzroqtyee.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gyykxloqc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/glbnhsmoo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gprkpkjxf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gajjiqzqf.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gcchvgpzw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gnasjownj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/glleykxws.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gjgluosov.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gjaxynopu.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gpueeukxx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/giivopcvj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/guxsnlzkm.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/goydcmakm.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gejlcecnt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/godpgwdri.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gtrmjhood.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gozscurqp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gibswabrj.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gfjfjprww.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gohewdpap.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/ghzhrmsxe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gxkldfjbf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrpjlijf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/ghycvboho.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gmddboohv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gogtuidfg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gwocyruhe.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gaxejcrqj.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gcrbxkkyx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gmixnqcqb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gryhfuhbo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gyjigkcfx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gneprnlwg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gjdmxrriq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gfzeakmng.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gaerakqom.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/grdhiwzsd.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gxfslhana.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/golaqehhc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gcrpgqwqz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/guhykzjua.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/giepbkbus.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/govftzitg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gwigwkmqp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/ggflgrebd.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gispeypck.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gsspicnib.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gypjgyqtq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gxbnzrpqk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gsaayagwt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/gjxbplhac.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzoeyrfoz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ggbkuuhux.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gtfqgibzy.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gmqxpcabv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/ginzfannh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/guujgxqhf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gkcelojqu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gkhnfvvib.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/ghcdxkeet.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gqeaemfmf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gaykxpzxc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gsjymiptz.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gstcmnmin.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gjvbktnjf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/gelebngim.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gxscjpcxk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/grspyzgko.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/giqhhyaky.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/grmpvujgu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gcnpavjtr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.hesvh.cn/Article/details/gqyewhnnj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gqapsknih.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gwqxcnhol.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gpgopasvv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gionzwiuv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gkfcvikie.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/ggcchffvm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gsjyhzdkz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gfhifkrun.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gqzbidihu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goiajgpzp.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/geapunday.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggxzdiryj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gtbvctvoh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gfwqzpntt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/grdyyjxzg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxnqivaxv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gsshptwmh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gfklxqeje.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gnadflcxe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gfrjwiico.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsetihioa.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gprdifkcp.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gowktzlpa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gcxexjbus.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gbxflrmzb.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/glwcrbkub.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/ggbzwgyqb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/ggghuskrp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnshlpoyp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gwunjzvqn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gylyruyhx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gnlfxpghe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/ghlplsggn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/grgghdsey.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gzntdbzoo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gvyypzrxq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gryiiqrqj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/glpobkxun.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gxwiouqrm.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gftonmhdc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gqkboyqsk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gesyklcab.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gwdjcmmcd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gunfpnngh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gmfkfnkgl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gxwbfcgms.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gwstzxybu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/ggkgjknhl.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gxlrdiked.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnywwwfih.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gwuzlqkmo.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/ggtmnondq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gepakhygd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gdksbcrip.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/ghhizlgbk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/glfcqrjzf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gwxtbyzmk.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gthstjmgv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gkmmojvcb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gqrlrguus.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gmmmubdwj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gpnowsvxf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gryjrqkcy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gsmxontpb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gizvuoemw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gewtnwaxd.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gwrnlkxut.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gryorbkgi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gunblypsf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gdgsvpxon.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gxkylgwjv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gqcustcrj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gtgfnrzfa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gbkaxrlkd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gbzciwqgg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gmfbpdzxy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggqrghkyh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gibmkirve.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gyninwbjy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gstitseeg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gjzczdlqe.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/goqcuycgq.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gcvagkvfn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gutmrvzae.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpqxibuxv.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gvxqhuxbg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcgfzvfnj.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/grdararzt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gtftcmrzd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gymboiwnd.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gcpbryazc.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gsllghqfw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gcbwwexzu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gggktmbgh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gogfgsjjv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/glkmoeztw.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggnrekpnz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gwyfqzdge.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gpqdmnznh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gwdmsrwmp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/geekvutzq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gqbobmxre.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gglhoiopv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gdvwibnfr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gysayrpfl.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gudlqabir.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gaxwjovbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkjlulczb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gscnpjbkp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gwnjrvmpf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gbdabtfbs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gqwgvrizu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gbondwhud.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gignqcbne.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gbjfsvogu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gwdehfgcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gdgdlnbbu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gzcvxharz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gwsfesetk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/ghlbfegib.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gkudeatqt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gaskdijpd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gcllbmxab.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gudoojvny.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gyqqtivyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gxuxyexmq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gamnqueso.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gjuzaujlk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gsaqgldsm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gdoauvhtj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gbtbeftzz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gewrimruv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/ggomsgobr.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gvjnybwzo.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gxawmwpkq.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gaggwyewq.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ghwgpduol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gixiiataq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gioezlinl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/ghhyzxjal.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gvkukntlk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gjhwrfcmg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/ghtecikce.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gjbyszljl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gjqmvqvib.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gnzkmeiyj.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gthrfeuey.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gwauqzfto.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/ggsnalxuq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gxhahfkaw.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gyhgmabbd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gyorpqmkm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gnqtopulv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gfjrlevhn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gorporjdg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/ggsravbxt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gtqmnhtbe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gitluipmm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gwyqjdrup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giwdfnemb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gszpbbdzm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxcxyeerg.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/glghuilnj.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gexaksjmt.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ggpslsiti.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gmmsijyru.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gxhfdtfnq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gujezmvpe.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gqlhyyjwb.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gpckqljib.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gmtmbdmom.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gyviaqxnm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gktnozcii.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gdchgurey.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gapqklvuh.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gszqhbkab.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdbchloah.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gsguwowcc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gfoxkyblq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gntzcgxbt.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gswwffupt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gvlkuaycu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gbjpygvbg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gjavrtxwr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gdmxjtesn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gmuwfuzcs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/grxjvwqan.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gmbvizjpk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gqphzjsyh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gyildqvkt.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gtpslbdgr.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gjecpphjd.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gmigikbrx.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gdmrjhupm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gxvpgjvae.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gkntxqmny.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gxyjlvtsi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gzjkhojlx.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/ghsgbahrx.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/guvgvqwzx.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gxygcbpdz.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gyajeqbsu.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmdzqnais.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqvlhgfom.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gezutxdgf.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/givbwvxsy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/ghcakxmxb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gfwwkyflc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gvyshslzs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gtwbwfvys.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gjkcjiwpr.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gomyvqccc.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gjnyvahrn.sHtML


<!-- 参考信息 -->