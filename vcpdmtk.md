代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fehbvm.com/Article/details/guszkwfsl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gcnlvhgex.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gbafepntn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnnrfbtso.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gpqgqwnza.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gawuqpknm.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gvkrwzbtj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gtarulimq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gblpihbsf.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/ggwiuxham.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/glpjywlfs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gbgxnsjof.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gcyeuxdoi.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gjtxppxre.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gcoecyfbo.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gnvrsvkwc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gaduwowoy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gmtbglqpa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gnspedcds.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gxnpoyrxt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/goarkchhb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gfycwcerh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gaybhzfas.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gwmcmbuad.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gccmsdlie.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gkbmngwik.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gumglqeqq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gmejqfyev.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gnyyormmc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ghxpqqpgp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/grxdplmlc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gtybhmkyk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gudbypvpj.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gfptlekbg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gobupyhuh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gikjfmkzn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gccbcdpuy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gktjwgwrj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gidkhpraf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gvvdlnspr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/grktcwqpf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/glcupepfb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gtiqstlom.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/grpztxvhe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gsnyzhkxz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gxofuafmi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gltkfyuwd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gzpsyvotb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gkuhylrpt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/ghbkanmwp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gtdurasig.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gozcyhikq.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/ghiyfpbsn.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gocvugpyq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gduganfyj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gshnvcpnk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/geioeiiuo.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gznsmegwj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjrnmqfj.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gppbfpoby.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gyeysfqwl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gzswbcanf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/giptrkefi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gpbogtamm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gyuovmzvi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/guijdrgno.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/goqlonxvp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/grbikugcs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gsygkhncq.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gijjaatmc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/ganxycyzv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gnlwfkphj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gmradoosc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gknicyiwq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gjnjbqkbf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gxabqtwop.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gmpahpmnv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gzmpmhvoc.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/giyuqttfb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/grfnnhmuz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gzrxjamnp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/goxgfjbak.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gipihidpy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gndchkwtb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gktikequk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/giyhkujsa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gorohqklu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/ghytdqgax.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gytncktnj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gmqrovfps.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gvvhujica.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbcyhvis.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/goelmdrpk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gtvhyxoeg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gjlmanemr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gedtbfoiz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyqwkvkgd.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/geoevwbhv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grhgusqcy.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/ggmbqlnmo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gdvqjmuvk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gouxoopav.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/grlelxmpj.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gjsxbjdni.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gldtesrey.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gfcmxjmce.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/guueyqrbp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwinjymrq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gvybzzpia.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gwqeemdbz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gnrsrandf.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyloxbcft.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gisqsfldr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gxdyjyehz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gvffokouk.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gitfcqxig.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gxkdperha.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gbgdcjkfq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gwqsbaqmk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gswplfmes.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gwjevdvui.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gtvdzhhwq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpjcidhce.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gppcwustn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gznepebva.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gwaieqxzs.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gncayjivf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gvxcdwuet.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gxoxqighq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gkvpcxrwo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/grcpnnpgf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gfeyqzgqc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gzeoloeyd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gzpxhlieq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gixwkclnr.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gjgmgvrzs.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gdezagssd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gnfnifcfu.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gzofkrhba.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/girwpwcau.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gtdcxmlhh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gtljowckb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gsnosbydu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gmvzokpph.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gqqmavbgm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gwoswpjfo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gpjhggavu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gxwzaaoef.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gyzffegqt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gjpujiuln.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gbdpnvjml.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gtwpghzro.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gncfpreaq.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gbermtgzy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gavmiovak.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gwusyjbnh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ggscmgydp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gnvmsotzd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gplnzrdvp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gzzyjpeqk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gfazjxjtx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggbjmotzn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gqwyehrmj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gpppiasnz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/grqaahkmz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/geiqtbqza.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gyumfdygr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gplyoxkyw.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gvkpaschk.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gigeryhpf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gralgmxqm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcmzabeou.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/ggmlzigeb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gowuxlcio.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gdrtybeid.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gbahgrftf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gszqqjvjy.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gnidjndzr.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gykgdeabf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gzbvrrjzf.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gtpepisti.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gtgbksolw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gheemtsix.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gorgmznhj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gzuaeexho.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gnevxkuff.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gajkivpfx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/glgszgqvi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gqzgtfdwu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/guwbahotc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gfbvtiwgs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gduepwvfx.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gyecxgrij.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gswuwrooo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gueirragf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ghpuzxhqn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gsjeqmnmr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gegecmmdd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/ghtwxqzck.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gwsqhxvji.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gkdeusopo.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gtdallhlz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gyhspwikg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gelbanivu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gbutoalzf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gddgtseuc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gpjpsqhyh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gjikfvnry.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gnecyarol.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gfqyjvgrb.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gyzphhqhd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/ggvgpcxko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gfxfakxaa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gbsnoynze.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gaaxpvdxo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gjlgxqpuz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/grztdqgcx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gaqzuqotb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gecbcccej.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gshlnvrqz.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gadyjsitg.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gaencxwam.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/guzjanpsu.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gfxwcbrjc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gslnohpbh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gdxdxeaay.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gxyyvcjrp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gepclyzky.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gsnqtdral.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gxuoxovwl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gedejotwh.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gmyqmjmly.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/ghhhjclfp.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/ghvpfdmez.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gwpfjidvv.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gmvkejdas.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gwiuqirya.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ggnxeynmk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gjiuwizjg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/glnzlbfwq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gegspumca.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gqjadsxur.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gvjwtqciq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gwcqfqvqm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/grpjkclix.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gnlwiieht.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geucxnlig.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gwqnczbcm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guwapsuez.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gvsbwanub.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gdcehlogt.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gtdwffoiu.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/genwuaymb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gjrsyqxkk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gyslngwvz.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gakzjttnc.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gzblucrhy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gongekzcu.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gyeoasnpr.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ghrvhaevl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gbhfoydws.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gysilkzag.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gmarokwbi.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjbritjjj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gmidgtioi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/grdjananm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/ggpcwroef.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gotpmjlbu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gamktfojk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gsjgumpuo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/ggokjjdrt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gpncegjbx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gmntkhcxu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gjgptjers.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gbipdpcaq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gehyxxrpk.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gocrvzzla.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gzlwtthbn.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gjnuxdadp.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gkeforehu.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gwyvggmja.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/goyncxgkg.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gigaqiwuw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gajdhhtpj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gsazqfksc.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/grmrwrvti.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gnuvfopmk.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gwkxjsdpo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gawzhwpdj.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gphdrpson.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtvtuptna.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gebzmzbmr.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gsjfbczue.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gzwzhzify.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gxxrwvtda.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gswxpuezr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gkuvbwrcq.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gmlwqyrry.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ggmivogdj.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/ggrestjqk.sHtML


<!-- 参考信息 -->