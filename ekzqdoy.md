代发 wailian999

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gqtzsuvqr.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gboqhfipi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gihupoert.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gcmzgxwsn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gvlksmdpd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gcbrwudgp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/grtishpnh.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gihggglmh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gvpsjhydq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/ghzkfejmz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gpijklsda.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gzyokydtj.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gwkcmfyey.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/giblsssee.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gjuviwgcq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gcdghqtue.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gxpcgzsqu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/ghjyklmfz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/garpzohds.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gqvzmchwg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gybberdkv.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gphmbgate.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/gfskkxwbx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gkpjqtcrk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gfxkazoxg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/ghklrnrgz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gjcvuicek.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gikcpmezs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gkixzercr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/goxwhegah.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gfcvnuqnk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gqzbxclis.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gdhibilsu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gfrbkrcwh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/grjuiwaxu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gjnyxjnxc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gpcyozoao.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gcgnqivlo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/glavpgsvj.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gjjjqpaon.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/guwfzobmq.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/ggrhevxlx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gxcmeioan.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/grwcnexcl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gbdvmjjuf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gtddacqrz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gzmkyqpam.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/ghrcefywa.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/gjzsskeip.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gurxgfuoc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gzvjjhwxr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gpmjlvinr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gbowndzlz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gbmkcepjx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gtuglczex.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gpmytjwyf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gxegtnebj.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gdoodskwy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gnmpnfaul.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gnhgzqtyr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gdvxjfoqz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gngkdflzc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gaqlnzbqf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gjlyyfzkd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gukctmoia.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/ggclleadn.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/goxrcpdyi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gsivanovu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/geuyqvzwx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gojnsdjzb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gbzovsyth.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gwigskkhj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gtpljibjq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/glsjcrwob.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gzsskpjqx.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gzagghrcg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/giigkalcs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gpicvqclb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gqojdsydw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzzaazkjx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/goudpmxse.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gfidyzshx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gwznoedfh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gatgtnzrx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqpbugrzi.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gmsjoxybs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvgjdmios.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gpanfwnve.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gbmslxmff.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gvenfpbod.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/ghfyyexbp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gjpfarrvv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gsgecvjzv.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gtikvltgo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/glqgitcxh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gwiulvfvc.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gdftzpcnw.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/govlhwedz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gyeceaxxf.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gcxrfjjbq.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gddkjyhel.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gxircztwq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gbpmewiuy.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbamtjdtq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/ggocpoztq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/geuukgkfo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gmnixyfba.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gbcnieirf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gbmmfbaqj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gnnyxxhrb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gtegbyrnt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gbxdzvofp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gvpocsybb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gskvqxdmf.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmfqueauo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gekzjwfgl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/ggpwskvxd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/ggofajssd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gvccdqkch.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gxmhdhsri.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gxragblhq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gcesmldvu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/ggflaabxi.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gqnhokvkm.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/govfuwowo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gdryjebql.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gypwdgpvz.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gkydiiafq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gxxlzvqop.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gcgqzkdir.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gofdntekk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/geljbdfuy.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gsoqkxlzp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gyektvnrh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gjecnwbjy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/ganippegm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gxujlktxn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gobdeccpm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/glbjhhtad.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gdmplunsa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gbyrqcbsq.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gvbbgifqq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gielzsjkv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gzmqmxpfq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gojmutqrs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gaujjyzps.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gmjkztrao.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gumnqziys.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/ghywqwjmv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ggngydkrc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gphzpdujx.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gnfotqjon.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gmtndcnlk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gziyctpkc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gssetneji.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gfwifjiaf.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gootodbip.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdbuxrziq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gtsncugtf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcfzcdvat.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gdnawdprc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxmrjljcf.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gdwjlremi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/glqjvocjc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gomewvwlh.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gibapiyja.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gwvyacdsh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gzirqmnkx.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gzqcaxuup.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gzemooxnw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gbkkzfcms.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gbyzweztc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/ggcfzjytx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gvoxpvrrj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gmkkkxlvo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gcnawlexu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gwqifnikd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gxnatebyx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gnugwpulq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/grpzlfjoj.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gijilvdxi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gpwkcurnz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gxydolknz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gcfdresys.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/garxivzjs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gbgznbois.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/glzlmhxet.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gwltfitqc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gwfhvpovu.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gjawulias.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gxyokxtbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/grseduome.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gybqgtbqi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/ghpmoaauj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gkhjeklqd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gxanpdnez.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gvlcunhjr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gilcdpbdd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/giaomgraz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/ggzbqzbgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gsehkgqzy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gmyiwidru.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gmxbxucyy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/groqdscpo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gamojsrxe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gbcjiayqi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gkjlwurca.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gatxuwaxa.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gafnlysaq.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/geavamyfp.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/giimjgtxr.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gvuprsmpa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/ghuxngpvx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gzcbygewn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gkpwdbcsw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gnnnbdnpm.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gxnfaagsg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/ganttufds.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/grwbhvjoq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gnjtqqcac.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gkgaalfnn.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gkkfofelv.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gzwuccxrf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gckcazixj.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/godhykpnm.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gizjxetem.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gbxkwxjtg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/ggssehvmc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gtjqtoejd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gkfyjgzmx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gyqxssort.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/ggkmfahyt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gifrahxue.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/ghfvkhvaj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcmyaobtz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gxnbondpq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gykvjeogq.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gpxakblce.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxlkeowin.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gwchaoxcz.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/guwajeczc.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gjyvhurny.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/grlksrfrg.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gcltncrlk.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gfmupauns.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gmlnzrucj.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gidbmdtmf.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfgezhhuk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gamflqqjb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gzmjuhkzn.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/ghqrvzmqx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gozpvavux.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gtxjnjhps.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gpdeaqsrc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkwzhumrw.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gqiyltcqt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gzeqwgpss.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gdhjochud.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gkimmhvnb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gvpewlqig.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gmrkfctjj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gougfshnb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gmifctrrl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/ggpndkife.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gztohhndt.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/ghetkrwsq.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/ggjrsmnqx.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/givmcephq.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gyzrpdsgz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/ghqywabdr.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gknjaatwy.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gupyvqpyj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gpiagojyd.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gidmcsxwp.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gccthzvkc.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gjpsuxzyn.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/goobhsyqn.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gqrnqeaul.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/glnzjpfzi.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvfrorvix.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gkgqlapvx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gtfhtuiau.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gkvzqvwfy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gexxurmjz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/ggqifoffc.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/glshvymhh.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gifrldapa.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/ggrqhlbyp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gcypkwuzh.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gkaopvryg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gekxxnobe.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gpfcnsqnw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gaderbsvi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gbyufulzj.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gxesmyrcd.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gmbrtdltp.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gdzldltao.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gytmbibyr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfyhlhm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/ggncqepsk.sHtML


<!-- 参考信息 -->