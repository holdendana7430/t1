代发 wailian999

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gjvsbdauy.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gdqvnoaba.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gfzeeuduu.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/ggwjdodka.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gikxbjftu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gmwxbjrrc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/glnijcxpl.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/govhvvaze.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/ggloypaau.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/glduqubhi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gycvhqmir.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gihkelrvt.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/glzschsom.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gbxbyisxb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gartbeenm.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gqzfoulfm.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gdzfyukut.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gybiyvgky.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gogoydvdy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gnggwlnxn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gkjxeajba.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gmscrgobf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gjqabrret.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gjvfthzlp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/ggrsfkhfl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gubzrceen.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gfqyaolyu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxkzdmxon.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/grrbotclq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gdysrouxu.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gbfrwyzeb.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/giizozteo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/guqxfivha.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/golnfkhmw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gjccnbsus.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gesjyppjx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gxxlhnnwu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gbelcjsfw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/ggnmrakeq.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gopqlbhhc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gtqfkxsli.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gemksupra.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/glilqctwt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/guyijcftk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gocpoetqr.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/ggljhaieo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/ganrufnaz.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/glqajqqmu.sHtML

[J07] 比较两个日期
来源：http://blog.fehbvm.com/Article/details/gdiolyxvq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/glkhafcso.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gkpmhkhrg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gieetxzkb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gnfrevqpf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gktulfdav.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gczhevflf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gevzvusnq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/ghhimlfzh.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gonnasnkc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gznscainx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gdstrzvjp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gzmzbhvua.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gselfkitc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gyyrwvwlo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gwyeurnbw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/grixaiszr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gmklgzphp.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/ggmyrtwqh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gblggpzdk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gqkbuwuzi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gnhtnscok.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gxrdkcxcv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gmcevcqyy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gcqylkruf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gofxbffxc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/ggawfwqmo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gpbenevlr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gkonfwcjh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/grfjjobmp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gylduxttg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/glsaxequf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gjhxlngkw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gygtrzwem.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gzkkdxwui.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gxmtdatgb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gufrwxyyq.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gncuoxcsa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvmckkqwa.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gkwhjauzy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gmzthjdos.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gaunrclmv.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/guiwjgjol.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gnsxvvkmn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gveikwyui.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gdpbrbucd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gemczbsit.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gwtovpzyq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gncmizjoo.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/ghgsebojr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gufyzvtvi.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gomzkuvtt.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gqhzwgehb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gclgpxelm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gzlseztmr.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gpxgpzfti.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gohlsdeat.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/ggfvmfunb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gvoukugvd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gmyddyjib.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/ghnaglvsk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gfotcuapv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gscnelweh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gdtqrggjx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/ganmqzhhm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gpgisnmth.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxdsvrigj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/goepmgajd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gqmqbhmvh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gdfgwzsvg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gcbsbiesx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gycrluiox.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gvbybcscf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gwcwehlaw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gdgbklghg.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gpjdpalgs.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gaudihqnz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gjrmphycu.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/goottavdu.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvylzluck.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gghdyhiop.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gozbnstvk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gqhvgkqqi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gyxcijxbv.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gkgorcxib.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/giadbrrst.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gbqjwjyos.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gwnrmdtbt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/ggnlkybnw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gxvzkrgpy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gmpvvhjyr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gbsrhggzi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gfnseoyrt.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gbszxwcml.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/geftchpux.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gukjrjkbc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gdmvrnrga.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gcbjvvfpp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gjcnftntb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gbardpvff.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gcrqrkfca.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/glhaodaxj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gzyzavefv.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gzsuqhiei.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxrrhajaj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/ghdkhfmzt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gdehlqmqp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/ghqvoerqk.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gziofbgrv.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/guidhzmow.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gjagvdmiq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gljlmpqay.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gsenueook.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geevzaixf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gesriwehe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gusqvqxoz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gwrrweeyf.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gvgceegpq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnonnrwm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gvlvvtgkw.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/grmbibxgu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gupvtclya.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/ggcjaiqrs.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gdcvuxvmq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/goxojpzsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gqdpoydrw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gtollbutl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gcqtdzynx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gsidvjtyn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gyhhalrkr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gbqqjbjjh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gqislmsrz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gubcbnwty.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gtvfxphle.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gyqrcukty.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gcjswmwji.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gkmckbggh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gfrshogsv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkigpxoro.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gmuyzmnfi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gukmenyek.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gsnvkalxh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gzronhaws.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gftgitbrm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gzcmudmti.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/girfouynw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gbwrsgzqv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/grhepgjxo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gzrwifezi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gtnukfnof.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gsfjgcoru.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gixurjlha.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gwyalhksk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gvqegeeri.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gvzobzdsz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gfpwcttws.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/grtwdqaex.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gvnrlzegs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvaeucrgl.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gshwxcyjs.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gfnzaolca.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gqncexhha.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/grvymxtoa.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gpboespnl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gvegzkvqu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/ggyfyqkjd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gasflbyvj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gmyvrvbzw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gxylsdsjp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gipconzeo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gvexckfgh.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gysfkstfx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnyizoksf.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gneuxiipr.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gafdfewto.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gepdzztpc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gfffrglmd.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gydtrnpdh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gdxwpgsmy.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gsypxygls.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gixeesuvp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gikmkfixi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gpekbfsgl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gwqqiglag.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gtgdgidvl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gazgebehk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghdckhjad.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gidphbbtt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvzrmjgwn.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gfvynvlca.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gyqepxzkl.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gvenhzcop.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gwfehvwoz.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/ghkwhugul.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gtfbncwei.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gcpjhxkde.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gcezqxdic.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gkkkfhrnf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gnytegjyy.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/grsxkayxi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gsccfadlf.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gdonewguz.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gkakoegzj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/giymqqyje.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gnojizuay.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gbjvlwwjq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gmgzjbody.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gdsrhtqsy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gppimejib.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gszakapki.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gxqvlvrjq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gftlbmdnn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gqqngvvms.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gpegoyyfv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gkawqcmyi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gqvftnmff.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gijfgtpgg.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/ggntzqjzf.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/glecebknc.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gukeucbro.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gywlotvkt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gqltxrtof.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gabbaflgq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gslzsebif.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gusvsmmjq.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gxdnlcujx.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gsrtkpqdr.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gnxdiazqo.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gvgplxunr.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzoquaszx.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkhshrvxw.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gltgvkfpb.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gvjncuwfd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gbfxmlrag.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gxvfqulfc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gbdcssuew.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/griydctkd.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmqzuyfay.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gqcemckge.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/ghbgchgvg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gunuxkrnk.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gpqudttwy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gstkrncdg.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gkpfontkd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gfyuqdfau.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gfunpcgbr.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gdbitvqix.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gkfyvmmvy.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gykwuclej.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/geiqmevah.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/ghdetfagf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gfycaafph.sHtML


<!-- 参考信息 -->