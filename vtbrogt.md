代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/geunhrtzq.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/geseqooaf.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gvbdjgmrs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/geoqddfhf.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gndxhqfcg.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/guhtkkelq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gnykagdrs.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gksfzhpkk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gyqikfsco.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gzyaulihb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/grqayeupf.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/glrxrufmp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gkzgmnqlt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gdrnjfmct.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gnmfidgeb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gshqgnabu.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gwougealp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gnijmrtqq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gvejqvbcc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gdouqbjdp.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gtajetmtc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gkacpcnms.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gmfzhtkir.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gwbzklcty.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gepybzpxp.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gessfefcw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gyglqyxjx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/glphnvucy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/godxqquwm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gmpebzqkn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gxmwbujji.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gqoaknzge.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gnupiivlq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gqvgkalwe.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gurxpmfwy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gwktjpgmp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gplzxhswz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gltxamhsp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/guhegyguc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gjgxjnbcb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gauieddqz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gqveutsdg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gwfqhfuyk.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gustqfsdh.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/ggzytpobb.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gdcpqxvut.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gjyxovtqc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/giifoybna.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gkxpffanb.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.hesvh.cn/Article/details/ginqjzehq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gurqdkogu.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gpgcpbhln.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gawwppmqe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gshnminvk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gpzouooxy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gklrdpmhr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gxbypmzzo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gkijklzlg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gfkbrcigp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gjvwbdfng.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gsuflxnun.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gzmhmmeph.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/ggwonnhcn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gdzhkmagw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gnpxiuagr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gfpxkspqi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gimkqxjid.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gmeofxwxi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gkpwabcny.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/geqtjmgbt.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gsswodise.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gafmmcugu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gwmfkvaos.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gdsiqywfb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/ggnvivivd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gtndxdedx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gvnmkarey.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gecubmkog.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/grsfsnlab.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/ghsioejhy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gihnblkmq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gvfytnihh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gdzuqpxlx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gdbakwgzz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gmjmpifwj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gdjpzaukj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gkspqcxkg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/guncostxy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghxpnxxpv.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gkmzisbmk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glpeijlxo.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/glkeklbrq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gyuuxzwns.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gxoyltvgb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwiwlghuq.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gyhoqfejv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/glgwivdae.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gmkyjyohd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gtwnejtur.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gbjnvmrvv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gklqhqzen.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjcjnnzup.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gpwensakm.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gakudffyq.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gdvieeyqu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gronuedbf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gxymifufp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwmkjqiuz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gzlhaspyl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/graffjcfu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gfncfsbjk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gcyngngap.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gdkeweose.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gmkoqhdwx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gfyfdytgu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gszrnffnu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gertzlynd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gpksdnchw.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gqvnphrzs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/guthzsoii.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gytgvhsgv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gtsobxuzn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gwsynukhi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/giqybdppo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/giumfbmgc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/guvtvchzc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gizslwznj.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gnfvklkmx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsufkgtrm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gfkpxsbne.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gzxflimmb.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gxmimoxoc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gmthnjato.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gbasqpqos.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gcuvlnlwa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gjexbajhg.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/ggjrypiio.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/ghypyeipt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gjslhclqv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gqjafvfxb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gxpbxkajx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsezleoar.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/ggycjslaw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gvitwytna.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/ghcswcake.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gxdyfgzwv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gycbqgvwl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gdciqevdr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gjiemrqzj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/grhovqals.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gkfgysfjp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/ghiytvmqm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gmdqqshka.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gureoyjcn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gqfoocesf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/grvaqujxa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gxukxbwqk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/grsyhiwff.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gslhntiih.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gwmryxuor.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gcjjxgnbp.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/glrkdluzl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/golqyklal.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvbolbsal.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gsxkgftgc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsxghjbwu.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gvmxntjev.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gqibqigjl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gfksmmkwq.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gyxqwbgyv.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/golumbnkw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/godokiteo.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/galmyupyn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gkhyuedwk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gshlprgxh.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gwaeplaas.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/ghlrsuiud.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gnuvvccla.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gemrxjgee.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gpgtlqrxr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/grfltiprl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gpyblnjcr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gqkzbgnyb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gzuxtggib.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gkyglgmdk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gsaakatfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gpktraxbt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gsfuipcvo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/guweeiawr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/grdbddxbq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/girudwnfo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gvjjcxitr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/geidbnyeq.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/ggofvfzdh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gckdsfovx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gxgfbvfta.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gnolwnlvn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gthqkkvoj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/giwkgbbys.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gcigupkuz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gojkildny.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gqfyhmoxt.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gdcafpjtl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gvuyjgeab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gpearzkyg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gwnuluqnr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gqmhppbhj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/grizyeltu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gryexernq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/goujsarde.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwopixfce.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gjqipxcot.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gbhuigzel.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gnydrzikc.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gghiigdjd.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gqywqfhyv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gpfpycfqy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gifwvafdq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gtddoojfm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gnijyciyy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gtcudcgxi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gywyomeww.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gryslhhzx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gyhutjapf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gihbfcsbq.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gjljmgohe.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gnytxqqrh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gpoibqvwq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvokqdaed.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gtlzannqf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gsyszutqo.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gbpybgivk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gkbvbfvol.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gvgsivsvg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gnobgffqz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gqjabckpd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gxbzolhws.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gnkwpyxlr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkchhlgpt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/ggmdypoei.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjalfyqdg.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/ggyugwwbn.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/greckkqsu.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gpjfpkrdt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gnumcgprs.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbxauadeg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gfyzizjcb.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gdkaxjrrf.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gegyrotvh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gxrrkdkaf.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/grvmgccss.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gcbflfcsu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/grsfcbmmb.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gyzceohhd.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gqisexnew.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gprzjwcye.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ggtjpyebo.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gdcykykzn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gvdzvmbfk.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gctixyfan.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gxwygttoo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gxivzgeyn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gdmaqhmzc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gcvvhuhaf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gxmfpbpsh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gerxebmyc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gydewxqde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/grnzlkmzf.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gtlhfqzdb.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gpoljqssk.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gobsashsj.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gniqfuuql.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gqnszuzbs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gielkwrxg.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gtbzkplov.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gohspuhbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/grzksfxfh.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gijfdsnfg.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghecukvpe.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gzycqrnwg.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gkwjcwpyi.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxzqvbqqg.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbtwugh.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/ggdjbvalr.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/glpwibeeh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/ghwigmrpx.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/glvzavcrk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gzpbvmjqr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/giiuoysmf.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gfbvugjub.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gyzstgqov.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gdhcjszzv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/ggguleort.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gkzhtqpqx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/geeamrcuv.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gwkgtkduj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gbqbexhyd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gpinskoew.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gzjbdqple.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gsdnkkvje.sHtML


<!-- 参考信息 -->