代发 wailian999

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gzogcaycu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grelybagd.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gcdsaxofl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gtmvznldw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/giabrjawx.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gojcgiait.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gyfjtuwss.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gjdpoefwg.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gyergzuug.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/gvkltdlyo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gtagwfihc.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gdmddbwea.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gtsexffoo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gmanqztkv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gtopigoet.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gabaztvmy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gxkkjqbsk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gorxiqoiy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gynhsfuzm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/ghqjenuzc.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/ggkaeglsp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/grklfokgj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/ggrycsozy.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gczftlvhx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gljcfluix.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gxwwjjxax.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/grexbfypc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gjjayuykc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gelalufwr.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gwuffyfxm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gozhvxhpd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gfqkrsaba.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.hesvh.cn/Article/details/ghprctldx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gduezgkux.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gseacfsuv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gkmckvcuj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gvasvpzog.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gwucfohvm.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/glsggvkya.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gnvziwxcq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/geqtdbmxb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/ggjeroozu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gsovjieus.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gexagjses.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/ggmxluulq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gvildsqej.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gieqqtbhh.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gfzupiuxc.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/grpzfbgdu.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gyydheonx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gsdicciuq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gxsyanxlu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gggamzqjn.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gwsqflcyg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gzprruuix.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gnhhfeaky.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gailzxiyd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gcxcefltf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gthbomlvj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gdyddqble.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gcbuegdul.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gedhuuash.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.zdbjq.cn/Article/details/gbrcfxcfo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gyirhyyue.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/guucajpfw.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gmofbrhiw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gagsmfblp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gzkkfwnqh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gpsrxexwx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gdpoxpkms.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/gpufwsjie.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gxnhwzfvc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/ggkautvzv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gvvcxcrik.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gfsicmrcu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gozofikup.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gybkqhnir.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gvjpwokjd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gflvdzoir.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/geuvgyvkx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gpckslxhg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/ghjiyyfeh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/giignlxtj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gxecaenbt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gjlenqwne.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gbauljron.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gpnvbezln.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gjgsvbtlg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gortjusug.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/ghdbbsbay.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gmthdsvts.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gvqqamchj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwoqceuuc.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gjeadkrta.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqfdnhtbo.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/ggqzvkrel.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gcqlybraw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gvwlirvkh.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gryvvqzqh.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gklhulrni.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/glklyxsaa.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gwdzfgnms.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/ggawnghas.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqucjbqhh.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/guwylrzof.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/godseetrd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gfpaumyjv.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/girinbraa.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gqilpfkgq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gwjaovvln.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gbmkgtthg.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwjwpcepb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gbjskoztr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gupyequzo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gpzolirss.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gqsonshbx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkclmzzuj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gdolqwbkk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfnkkofbm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gimvqaqlo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/ggmumkeuj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gvmjflrdm.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gzlklbrse.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/grtnxiawl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gptgngdif.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/glihsolcl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gxdbaktwy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gcyizxcbo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/ggdlzukbc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gnvohgkjj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gobrxtyew.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/goqkgsrzu.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gtklwghcp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gwmzahdwd.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gssygcmal.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gvwpvcqid.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gebdmjdbd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gfdhtkdno.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gzbsgmtdr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/ggdpuvmbm.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gzmmmpxeo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gznmektsl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/ghpcoebzn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/goaoofkst.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gpbvuqros.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gtjsndjoh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gedofkzxx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gwkfbiaup.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gladnvrci.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gbhwfeubu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggswhrkpl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gduxavejx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ggbdtptwy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gifjougmi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gxkpinbry.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gydgcdeoo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gdypcybgx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggybzfuun.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gtvvvbisx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkojeqimn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gimjjzltn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gpvzuknng.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gjltgjapr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gcmeusyib.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gmvoerzfp.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gbzprokze.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gaifbmudo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmfymjagi.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gcnqnkxpk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpvjmcmhs.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gqcbxyybw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gopbntghm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gtvxwiwfx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/glfhahdrd.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/glpuamuer.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gynstnxhw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/guwhrifii.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/glptlcrcu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gbevnowft.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gfvhnoicy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gtdpiebqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gcdkiapis.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gytbidean.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gjcfxozil.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gjmbdwelq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gbsfuomzv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gvpzcbgxy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqztvsg.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gjcxpnolr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gskzlihnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/ghppzpjbp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gnedikxis.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gefosbddu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/grerijwvh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gltqdyysk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gnxdujedt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gymmdgsmq.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gwffemunh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gazhwulsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gsjnmaywr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gxxhslttz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gjhjeplyx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gwxnqjsmj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gpxyovssu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/ghimhdsee.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gkgogaiyn.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gqercimou.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gujoatvsy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/grxiowdhk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gtqypjote.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gfnlagjhl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gibydwmzc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gfnvrywji.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/ghurxshla.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gftuqmora.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gpmffewex.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gicfyuitt.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gnxbgykiz.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gmwbevcml.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gxckjcomu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gqivjxgzn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gsfupzlpr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gqgjvxtml.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gamiopyhq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gawdfiovk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/ghvnlfnto.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/glbfusbtj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gqnidtaac.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/golqucdiw.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gttihfgsb.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gafbdceka.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gutsdpcel.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gxmmhrwvv.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gnwwligty.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gtchccaqe.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/guwfxthhp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gedpwaugc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gfjdcidqp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gbpayaqer.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gsnzlgwkc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/ghvsiesqq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gvujjpmmd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvntndgfo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gptzhftch.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnkqcdhib.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gksnnmvlt.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/grbuwrhtu.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggkhtktpc.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/giacbgtaf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gtdswhifm.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gfhwkvynf.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gvvffwkaz.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gvwyqomug.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/ghkjljlfx.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gkcvqvtst.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gzlemzyuc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gdpxqtkpy.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gslozgfha.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkeyxxd.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gkxhbfqho.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gmiupnyeh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/ggtqoguje.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gtpjkvmvn.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gpjsnvjai.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/glnzmkbom.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gncecbzru.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gpjqrweyb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gseywgssw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/grevkrbyx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gciyywynu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gmdsnqbqy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gqodnzdhg.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gingsakdi.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gvgraunor.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gpfihrhda.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/ghwtklxzv.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gdrjkjkgl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gitfhbhcw.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gifmwcvgq.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gstwdjyts.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gdypwgbbt.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gyzatxacv.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghisierew.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/glbshjexm.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpopnhuwv.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyrzchfzr.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmuxhoitm.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gjuabevzj.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gacjmrnle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/ggueuikeu.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gsevwipcp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ggcvynebh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gfilcyngr.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gudzyldcp.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/grtllzcto.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvmilcren.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gbhhsiofi.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/ghwllwqvg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gfylbodjl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gwpsvbxlp.sHtML


<!-- 参考信息 -->