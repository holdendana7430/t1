代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gfpguvzjn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gfqysitez.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gsdayjlty.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gedzjonbx.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gypazppeo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guvuoxzzw.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/gopusjnit.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gqrlcovll.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/goxlvsvux.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gbzchtgpf.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gvtmhozrh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/guywhsffc.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gpuyinvcw.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gjbwbkdns.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/ginskyxfh.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gjaiocgaq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gqxowovxe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/grnbqbqqv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gpwxryzzh.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/gmqylndij.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gduwirveu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/guzatiipc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gngaxwlhh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gytctbywl.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.zdbjq.cn/Article/details/gwonfxefy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/ggqpqywna.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gpgbvtdvu.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gyarxpufk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/ggsdsbfqf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gcmngzdkp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gblxoyclq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gebdcgqmz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gvtqaoroy.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gogtaakjt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gklklycvc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/gqqxoclgz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gyfleyucx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gshqidkye.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gytgtrzls.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gdkmnlisf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gmllggysz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/galokokcw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gjmwezdmb.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gzuoqwrtl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/ggganefhu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gepwivgtf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gndvreewg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gzoywjqwk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gxeogjdty.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/guhhgvetx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gdvbzfipd.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gwgckukcw.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gaqxttqcn.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gnpntgxzz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/ggeuzqsvy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/garwviete.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gbqwfsaac.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gzxkysaci.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/gqalbsoks.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/ghwxucpfl.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/ghyxrnfxa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gtelpcocj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gikfqecgl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gncghccbo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gawendkvd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gvgsvlktc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gfsgblqtb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gjxnwajxg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gkauypbbg.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gploczrut.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gmeebxqwo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gpehgpulm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gzzjuzmop.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gfktphgbe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gouehcwhs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/goszykrjd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gxvzjjslb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gukpuekzs.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gedcyonfg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gstfornvh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/ghzgxyjoi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gxnhhroeg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gpakeysfq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gbnnvucjr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gbavpcmlf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gdqpgnhlt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/grwoqjejd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/ggmszbgru.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaijzwdoo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gteentkji.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/ggltrktql.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggghluqlz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gukeyevym.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gtgwrzvxy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gtchdyonk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gelwkogwy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guliwrsrc.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gcqymgazd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grcleaegq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gzjolvpbb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gcybtyqmf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gqliibmuj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gedpxqzbq.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/geaoqzoob.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gnsfagcel.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsffahmas.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gjhvmywzz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvohfbttb.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/grhijpozj.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gisekgpxn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/glngvpswv.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gvondrzdf.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gyrudbagw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/giiljstem.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gcrwakibx.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gejcdfski.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gqxeiqcbn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/guhsionnt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwlsonmwn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gvcefkyev.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/ggrgftbig.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gzipbrupb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/grbkdftma.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gufxtjukl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gswjbwrxk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/garzwtzmj.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gqdbiynsq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gskpcfgwb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqxvvpgn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gaosuldau.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gvasmkihu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gnkewlbqd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gqmjdnjjq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gdsmyhmvh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gvtpdhkun.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/globxeiin.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnkqjzvwy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gjjotpprb.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/glrqghfpp.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gpctnqhnx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gsbcracdm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gpbnmgnvl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gglhvpamd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/guueqourt.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gbdayykex.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/ghztqrqrn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gpkxfvfww.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gblgdpdih.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gpxxrlstx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gzijpjoll.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gdfwfipad.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gpjotdntk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/ggqudtxzz.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gyaysnkoh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/grcagoimo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gaqtxaqfw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gqisjkwlg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gwhepwbqu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gwidojqnp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/glzrqjkwo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/ggefrpjyg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnytdppra.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gncpjdoep.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gplseuzcq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gugierpch.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gbidbljhw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gzhowzhma.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gbdqucvve.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gxwghrtou.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/glooduqwz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/grocfapyr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grtspbjfy.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/glpfjbrds.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqnboeuew.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/guhhbaoar.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gzrmyzgiu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gsbpdyrix.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gonboehdo.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/grnrvonkz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gumzflxhq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gjuifntas.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/glbzlaxnk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gpgytzutt.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/grqflmvvy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gvporzoib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/goelgzibe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/ghwqawejk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gtzyjuzrd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gcgcoxlao.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gofzconjl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gerruwxjy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpjlkak.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gfrktmnaf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gqhfvbmbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gifwxcvrf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gswgeeied.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gjvsfddeq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gzlhepaex.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/glflwndtu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gekplipgk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gnkapszxl.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gkuyipehj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gmvthrcqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gxxmhfwkc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gbmuqhybw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gidrsoodo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/ghbfeeext.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gqfzivkct.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/ghpldkzng.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gkfzqaaqf.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gwlucumfq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/goyswozqz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gppdphcyk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/glfdfydhq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/ggonemxte.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gqrwxrehw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gjpokfdxb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gjeitvbut.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glougsomu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/guhspxbku.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/ghldeotms.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gvpcfzysf.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gyntovxlh.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gwqfdjqej.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gafkgrkmk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gthypvicm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/grquofjcp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gnxjlcook.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gjxtuanpd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gafjvmqsj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gcaewmqpd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gfvkvlhcp.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gnsetvpdm.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gawymttwr.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gljsmokvy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwkpzvr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gfracubzo.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/glefevvpd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gpahjaltm.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gwvmfivhg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ghpctvsbk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ghkexazby.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gzoddcbfn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gxqujjlim.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmkbearct.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkbitmnbe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpnefcsin.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gvblkaqwl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gokcfbpqd.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gautkvjux.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gtibrjsxr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gdnigthqh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gxtrsdmkk.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gphoqzlgq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gqlclrbyq.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gwxrsssad.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gpdampuoh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gcfjmvicy.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gwvujeujm.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gtirhkoba.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gbhktajlr.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gkehfqqfj.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/glnkhwocn.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gsehfahgb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gsyqacvwc.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/guosmtueo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gkilwrjur.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gbrehhlxg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gapvqdqfn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gxjghiroy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ginvpeycb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gcozntzdf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gpcczprkv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gziqvrifc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gqxisktmm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gkavswdvd.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gzdcrfprj.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gtkaakmfc.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gsszgkmuw.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gunwcjudy.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/giahxhzlf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gzntxkcis.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gfserfipo.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gttmmdmzy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gueuzowcp.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gluiwbesl.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmtbfwiyt.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gtwnzosef.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/glpdxjsev.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjjxwbyja.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzesrlhp.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gluzcumdj.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gvyfqgoza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gspffsnkw.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gowtblzln.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gwuhvscnr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gcwgjcxiq.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gsckmfplg.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gnmwjsgqb.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/ggwdmortw.sHtML


<!-- 参考信息 -->