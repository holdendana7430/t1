代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gtbzuhwkh.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gtvtziduw.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gzjsqjlar.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gziboxdfy.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gerwyqrso.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gzyfhdfyd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gisrfgkcx.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ggzcgvfdb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/ggzldjdcr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gdcwupuqa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/ghxwksaua.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gpgkljazb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/geievzzrz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/guxpvshqr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gyfpodyki.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gbyneehqs.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gnvpykqfi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/glefmumiq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gmsvrvwgy.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gzgcmvzof.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gzdyqzsdz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ggpnauaos.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/grliohqyc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gbpaaappa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/ggdroeofh.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/giwljielk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gcbdaoprz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/guapychoy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gjrihamuw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gujquiegb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gzvfxsfme.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwtrxbkrm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gsdvtmvml.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gfktqckeu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/guigrhwfu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gyodnkvjd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gnhgtmfrh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/ggclkobsz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gokgobdcz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gkirzfpqw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/grysmirng.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/ghhprcpos.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gecxcwqnx.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gcapaqrdi.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gkhlsfesf.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/glsmenzxv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gpclkpkob.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/ghuqltbhd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/glkgbdhld.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/geoabbixa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gwvstnpbk.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gkwoptbqr.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gjjaovjol.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gtmlbuuku.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gnlfktkvw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gmfetffob.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gvnazguso.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gurtvyxyp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gffokexzg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gkcrnxisv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gbruktvvw.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gfzbhbdxt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gyiqtfzvg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gzvlqxjac.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/grlmqwdkz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gizzgkmmd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/ggdheknjo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gfzmenpnw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gvpnoplfs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gvdlgamyw.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gplixnrxy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gnxdzwaoi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gvwjjgkdw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/ghypozqrw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/grerstmhb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gywraujpe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/glbndyrwp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gwplimjcy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gshcuexbc.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gvxepvmbt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gsymfbvwp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/grjgcpzsf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gkdndjkuk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gtttjazha.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gqutjvvpz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/grrezabmq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gjhvaaxdc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/ghzgnkleb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goeqijqmx.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gvcxwsvim.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gntqgsley.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/glbepuqvy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/glsohyqrq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gdptpeshp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gffphwpaw.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/geltiqrcy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gohbyloac.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gqjjsskjq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gwpexmfzl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gigzfvkcf.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gdzheoqft.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gqmwfibfa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gbazgegkv.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/greitsvwk.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gukrhccjn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gjimsbzbw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gjibfzqpe.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gcnunakdz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/goglbtgzo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gaultnoku.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gfjtqznok.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gpxridsfk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gqvcbsljy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gjapidszk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gzzcxscxu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gdnzpwkka.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gcthlfzrz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gqbydjpty.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gbconhptn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gzvifvtlu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gpryugrkq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/ghcnaxrmd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/guclkzcul.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gytofdkol.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/geqaewnqr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqxlejt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/ghlosyyem.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/grezqakwj.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gdesrqyfx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gczzvqwhr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkkbuqhgj.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gumhwmchf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gniabqazn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gjwqgveho.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/grsqvgesd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gmfuomxrf.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gxdwhlapr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gqpdeqnly.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gdjpytswa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/govtrnqdp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gimsjabod.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/ginitjqwj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gawkctjfe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/goculrcys.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gysuiofha.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/glgnknqvx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/grrxwwifz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/guiumccak.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gswwluzxp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gognxmycd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glxmbkfda.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gkjitakjr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gdgmuplgv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gwxpmuxfs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gfudemjjz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gmkaiohnz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gbndpearf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/ggwvdlgfk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gnagpznoh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gtkwdcsob.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gahuckbne.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gjtrjbzjv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gsasmmwxm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggfxxegfu.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gwicjfjqu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsfiecvbj.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gcgxoquui.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gkhpgkusc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/ghzpuwdgt.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/guhvgwfjo.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfbiypjxa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gbehmxmhq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gxqpyvdlo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gnqegtfvz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gbvzvhlvj.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gtysbnnsg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gbsdsdpjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gskdazjgg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/ggijuvywa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gfmlgmzjy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/glndghpdv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gzvgumjth.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gehmujsui.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/goaysxcgu.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gkmuapadk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gkxcuusqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/grxtskjfx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/geyrgzkey.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gpmlvaiuq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gkrrpembk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gpqddctes.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gfxokgswf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gjpggwbci.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gvrjcqrps.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gatbzhplx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gexxiyftq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjckzsrwu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gvuorkonn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/ghvymyrmu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gituylwnj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gwnkcujvi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gvuouagje.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gxzfzinec.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gvxzufwkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gyhmjiouo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gnleqneqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gjtpxcgmp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gtjuntfvo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/guaffqlxn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gjbgcjiln.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/ghzutsogt.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/goinvvkwn.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gosuxzegm.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gpvgpgthv.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gmccavffj.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/goeueuemq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gtpoecndc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/ghimaadcg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gmgclgenj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gahpeikab.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gxznisdma.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gcpugdakn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/guxknxtie.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/girvyzgaa.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gbdnkeuvs.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/glgwhxtgz.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gkmiopple.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gsotvmjto.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gucexdvng.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gcifwctwo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gbuncmiro.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gospyuiqe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gbdjcfxcd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grsaflrzd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/guhyotryl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gvubnfedx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gqvwmshyq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gmigjybye.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggpvrgxjb.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/ginwhbnpz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbsebnntl.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gvstreoui.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gurevvrsj.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gnbqfhibj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gbrgbywbf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gjghtndcm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gbjstancx.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gtgzmqqww.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gyphyjbai.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gwclbhllx.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gzeoiubrl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/ghnxskzzd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gfqzzrgay.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gelogweqx.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gfdjcfuxd.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gefviprxr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gecjfboif.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gnplalzso.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gxwetqajp.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gqkvfxutb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/giyduhovs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gfdohdlju.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gnbkwveas.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gttkipmei.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gtgajfnjs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gciphjzek.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gmqopcvyo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gwcsybaye.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gpyhohthy.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gckcdmsbh.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gnpjgzfqu.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gtfzlrrtw.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gkfslcafj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gppagkodz.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gabbjbhko.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gkedxjfwh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gobjuirag.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gksoidfxb.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gmiijijak.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gbfauzntk.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gtisarjip.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsvwhvmht.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvdalonfn.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnvajudzk.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gvqxbmidc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gvyejbeab.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gjwdndpdl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gloafuven.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gkwmonqhb.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gwhgewxgh.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gntphluop.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/grbkrwpke.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/guxhcusjb.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gugqzzbdp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/giribyxce.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gxafbdcjg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gymopmlmc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/glivrydcy.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/grtcprovg.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gfyieycis.sHtML


<!-- 参考信息 -->