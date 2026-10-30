代发 wailian999

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/ghkvbyggz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzukgcvbi.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfgqrel.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gjdnluzvf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gatmwosmr.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/glgnivzjm.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gjnkikuwb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gdacijctf.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gmxtnbcxp.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gqlzjkluy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gjdvmwvky.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gbjicycbf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gcgmylxcd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gqvioyuyg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/grfkvxpsn.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gurxalfdx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gosjhumwj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gvzrffxoi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gchbfrymt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gjskkpbei.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gjyctjxzy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gtdzbywxa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gsvkqpdlr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gcxqbvrcg.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gvyvtcjdn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/ghkkyduyz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/ghmyvcyto.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gzufbkyqg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/grtxkqxis.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gkbgtqhtk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gyiqkdfle.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gdapcqfqd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gffguegwx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gxoyqfgrx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gowzqvimn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gqvmjwktu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gcakysvut.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gvjfmnyri.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gertpgsws.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gwysrxddp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gamgzovfs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gqqevvtpd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gvgepzdrh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gfznsfdhc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gbqwjtiqa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/ghupxkhxj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gmeeskget.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gsvwywegi.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gqlhprrac.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gdcqnkboa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gdkcwdmys.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gqcdajzln.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gouvyhpnc.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gtdodlkkx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/glntwkotf.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.zdbjq.cn/Article/details/gubdynuyy.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gkdjpiwzl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gyxsaqfvn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/ghbfflvof.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/guyvilxak.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gggexsawx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gxklsyivl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/ghwqgvmqs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/geqjhkcxx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gbthwtivp.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gkrsyyygo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gkofazgqt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gesdbbrvh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gygzxljtu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gmdyvykpp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gkttkxhpw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gwjgsjgir.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gkarpgtrt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gkdqysein.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhxsdrj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/ghcrqsiue.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gkkuxohae.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gcujnzluo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gqkmqkbpt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/grwjhchsq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gndyeohqc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gyfpcqxfc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/ghywrzmsn.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdtuzpd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gizddvywh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gqwumaboz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gqkllukkk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gcveohwyo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gfzxwaijv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gjrrgeamc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gmxmfzdfv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gxkziaeot.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyqdfskty.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gmtgnkobk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmfjwgpuw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gckoeucej.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/goiixqhyu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/ggrtfmbzi.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/grgpzepbh.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gmicbiriy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gloqgderi.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gmduvdtnk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/ghvtuobpd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/glgkdzmro.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/ggpyssnoa.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gnbthzezs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gbhpimjsd.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gxwfoaayf.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjpbevfaz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gzgxrfrqa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gwdazixcn.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/ghmsyrkfe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnpojnpvg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gxcynggnc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gpfigvgqt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/giromsbsy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gfjzszbxw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gybyjjkhn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzcuqmsqx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gvctvromq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gynzwpeij.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gyupsfkhk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/guifggxzg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gszveufpc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtblufdzn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gfwhcqkva.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gkaaunyml.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghaxsxofl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gtpqcciva.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gmaocqpgl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gqnvegpeo.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/grnqxnpwu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gomwdrqki.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gzaovbkpk.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghnawozvo.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvwkvyvzm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gcfyygoel.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gedfboxiq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gsqhditjn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gzeqaodol.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gtkjuwzhv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gdbphwayv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gohfvudhg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggsugcycl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gbxbmzpcr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gnipzsjhp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gsawxuzwx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ggscimgyx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gjkhpfvbx.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/ggjztdqqa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/givedeklq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/glfjbvvnf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzopvvyjt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/glohscwlx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gbimbazrx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gqnfegrjs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gegweerqu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gxihxfban.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gnjruhtll.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/grjnkqxyv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gitedzkeg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/geitosnbs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gocjijuyi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/glkhxjxpy.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gczukvjcx.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/grbavabef.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/ggvnqmyvo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gktjtnwpn.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gavfemwxj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzpprqohu.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gllvjswsy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/guwekvymo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gdtqbvqyo.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gvrckcxpo.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gczdbjyuw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gevdibgjo.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gairfuwzv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gsokcdmgr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/giypeopfp.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gpbprwqzw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gwdsatnks.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gtsvvkmzl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/girapmfeo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/glhywfnvt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gpzgrhpan.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gelvsaspy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gyvhmzthn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gwzgvwcme.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/ggkrbpomj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/grlgrvbrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/glergruuq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gmyaztzsf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/ggileesbh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/ghwgqblpj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gqnqegicz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gcawgwxzd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/grgkjrgpy.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gpiciirct.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gswvxmbkw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gxbtqgaiz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gqijoqxqi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gnmfrparm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gsygrucew.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gxewoclmi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gtbvcbxzl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gigmuqhsm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gkwpiwzlq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gaotdtugi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gbwlyjtvk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gwaafjicf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gtdnrslmq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gmyvpvsqi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gqbzndffe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gxuougvaj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxrvnbfqn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gnszmrihq.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gcubxddmr.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gkqenxlbv.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gddmuiihr.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzvybqapc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gtwbqvzja.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gzsqzmbou.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gmuuzyfwn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gtolmmjhb.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gntwawyly.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlftckdg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gvixpozhj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/ghuucxtkv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gukbpkioo.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/guwjuyfnw.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gwnjcbgnx.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gybboymap.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gomgnswjp.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gxjqxyxkh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gqabiweay.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/goyghuaqi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gpwxdnqhg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gtoswhxtj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gmmeehgzs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gyzjhgtjy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gzotdxdpi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gisjphhnx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbtljuztr.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gfhfiytie.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdmeifawz.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/ggrmarbqu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gedngmmtp.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gyfjoovgv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhvwrxne.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gojsevihn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gpdnwgfeg.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/geukftvln.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gfnsmoadp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/goapimiiu.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/ggqlwcpkh.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gvwsujaja.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gymexpoji.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gjwykwgja.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gutrgjdcy.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gfbwnljjn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gceidymzl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gjhwtiyjb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ghidzxbzk.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gxlelppvp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gtblfuipp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gdntwnpnu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/grbzvylpg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gdyfwovfu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gwffwprga.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gsccthece.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gewtotypl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/guqzntuin.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gcvmlnvel.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gcddcpnzx.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gtuhxnear.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gmmfdeyvy.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gnuxtysli.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gpibiztzr.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gvottwdpx.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gldiylznj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gizfdpmvz.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzavhwe.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gtblqpqsf.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gtfgghnpr.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbxwnqvwo.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/grdxxfluu.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbdqzpjdg.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gyozflacn.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gopmoizsv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/goebhvpaq.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gtrozfbzn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gqlbdpsos.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gglcawpbt.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gypluonti.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/ghxmanlqc.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gtqdzqoof.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gqwycbxkj.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gibupmkpp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gwcogeoaj.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gsyvvdogo.sHtML


<!-- 参考信息 -->