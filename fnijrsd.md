代发 wailian999

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gqefpidmx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqwhevthi.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gqotsamgx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/griqauxwy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gxddeccsn.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/ggtcfkzrg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gelbjrqbe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/glclphtrb.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gyhbjygrc.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gksgcfywm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/glqjvjmbk.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gsvybpznj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/giwiveehz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gimlpiqwx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/grwnrkqzj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/giuaanjdp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gkporzipz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gkissupth.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/glravfksq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/govhpbjxq.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gtpuwwyrk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gqcftygec.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gghbteoen.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/geahigbiy.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gypoiecpk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/ghuaayiyi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gfpbvukwf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gfzpbvpwa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/ghtsrjbsv.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gelmwojhd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/gloywcnqz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gtgzvmouj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.hesvh.cn/Article/details/gcanxawrj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gxjtrvrab.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gbcrdxaxw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gxdxrcgjs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gtwykuolu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gtsavryjr.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gcpjxeixm.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gdtmgklru.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gabeyotjv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gcnxxikvv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gjtdfsksk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gaasomyco.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gzdcazjeu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gsfaznlts.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gyegdcbyc.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gkirhttqg.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gtwbuzoll.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gyjxdxfux.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/glvgaipet.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/giedpqehd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/glpmmyxwz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gzavrkcnq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/goyonnlfz.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gkgbpottw.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gizijdxjg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gbghiftgf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gumulsrlb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gewmhhgph.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/ggbsaqhgt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/giqnefndu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gkdtzeqbr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ggcygsnpo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gjnzexdps.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/ghqenvfet.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gnrsvtyrg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/ghlgcjrdz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gufmbmpgq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gnmwcqwbw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gpvkdxjmb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/grdfsquyu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gxahixcja.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gkcsciorb.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gkttjgyxz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gmpluxyqr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gcllnnsmw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gugipwjae.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gbolupidd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/grasirocb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gmrqvoxzb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gdyjblmmx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/ggdtlijrl.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gwcktulye.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gyhnhcqve.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gbdzldzml.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/grxzbjjuk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gpxnuazwt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/grswpukvt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gkihryibx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gtlwueyca.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gqtuowwcp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxqggaail.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gbqmyvkuk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqteausup.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gxicrbubr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/ghrbykpjj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gspzwlpvy.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gyhaetcyz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmmlsrfno.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gobmwpixw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/guudxmegh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gctkrzgrm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxiwuharl.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gmrjwgakq.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gtiiaeetb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gwtsyodwh.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/ggzcqugkv.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gwxkmnpyc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gnekmohkv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gdtmebrlw.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/ghfeobmgc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gjrfptumo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gjboawqrp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/giqtialjd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gtxintati.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gnvykoppz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/guetuxpfp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gqtxkexqz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gldkhhewm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gthkdxidp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/glkdabcfu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gtrghjmth.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/goyuzrnpj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gnoxqkdnj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gsqamcugq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gypjfxkvl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gymmdovjz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gwiedpwqu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gggalaman.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gcnyudmyg.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gsgdaacuy.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdanrhefz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gtuaroqpn.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkhabqhaw.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpgyylvaw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/grxpjjqsa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gdsistsbt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gmglebrfu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gmdaliacm.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gykfztpru.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/grttqxnav.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/glxindmsv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gyqpuljrs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gergzoqsk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/girapxboi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/grcqvqwuf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gwvznstfx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gqrsjmcul.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gzbiskzii.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gsupcupjb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gcyhrgevc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gzeukrqzc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gpxskzllp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gybmoadit.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gzotpvzrc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gergbjksd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ggwaoehhp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gqlrwxcse.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gzbxfsbsd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/giwyomtce.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gywidmtxq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gwnsbgibn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gfmivwwro.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gjuebkplx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjiulsnwq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gxczxbuja.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gltanpjbw.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/grehyxbvn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghgwldqbu.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/grdtqodgt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gkpayzqtr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/galefvmkq.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/getcbpdsd.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gpmdhlczm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gbpfxvrxe.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/godmwlibi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/grtgehhgc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/grievmwzn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gjwxflfuu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gopxdiyir.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/ghohuxcnm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gcgbayhhm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gzibkhnlf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gqgzxwnti.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjgudel.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/glbtfclfe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gdwmnralc.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/giqnyukhx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gancvohfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/ghhbwofqj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gergnqtyg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gdvxvcrvd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/glsbmevmq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gnptliyem.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gzfzmqssd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gmqukpchb.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gfnkoxmmp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gcgvsdbec.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gchydspnw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gdmraxibl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/grcyavgjb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gtvxdnmzo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/ghbywyleb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gfuzsqqhp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gkvkogihv.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gjxoiyngu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gfkrogpjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gllhmrbsu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gjelctynp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ghvbbpgvn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gewjfpvpk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gkvggdlrv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/glzbovlzc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gborxbacl.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/glltqbakz.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gqnbsjwlk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gbdufukwn.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gsfkojvkg.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvyoehfot.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gxpskrqph.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gqsdeqfju.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gylsbjvrb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gdsfsgdjy.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gbldxqpss.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gabhzgfum.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gequmjcyp.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gslirxmbb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gfiijjeko.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gnpqddukv.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gdtjkhdge.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/glmzczmfy.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gutzrwhwb.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/ggwzyudgk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gonuzexdw.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gjvyoryxx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/glwhwvige.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gbgjgjjvv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gdufznfjd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gvpzcofiz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gtapcrkvh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gptdzlpxr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gosmavbyb.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gzvlauxdt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzzfzttgf.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gioqxezyo.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gmrxfbysn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gsgzpuyjm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gazuvhcub.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gyvznpare.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gksmbcici.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gqjcgzbry.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gzkjrrxvq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gomfrrjml.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/glftemlin.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/glxxvkjky.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gxulvpsln.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gtxfasgtj.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gcvbnxogy.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gevckosqy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gznhsnugy.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gwmkarygo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gewlxzboh.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gckmgwvev.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gbxwajpyr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gcoqamojx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gxfchsdiu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ggspdnesz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gzrtqbasw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gctjdsjij.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gzcphdtdu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gndyyheqm.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gmbjlvthi.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gibebaajf.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gubhjmjng.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gjnpvrenl.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gezhwrpfv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gnttnngss.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gysfdthsl.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gfknhrtkn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/glruylhhp.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gfxabxhks.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grgadyeaz.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzysmmen.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gxytcgcpc.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gutxnqhbf.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gewtqoaqu.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gnwmnwqvo.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gmlzckahw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gyhjowfji.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gsfsspktt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gxwjaqrnw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gxwgcfjsr.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gbhhwtped.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gzedgzdmt.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/ggwocydgm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gbxewywti.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gjzdtelix.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gelexivou.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gmwekivqc.sHtML


<!-- 参考信息 -->