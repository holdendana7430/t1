代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gjqycawnd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gnlvrrprv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gvbctmsfk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyikrfcrn.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gqbhmubqa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbkayihfp.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gbusgcfzd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gtaoxuojm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gebuppbkz.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gnyipufhl.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gspseadzd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gqyzxdfbn.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/ggmwjbvjy.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gtyvsmgku.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gllenilxm.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxmwemwbu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gkdujvfrr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gyevvdicg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gecyabzrw.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/gernexzyf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/geyktkpqp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gvykjpzvr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gsavozfwx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gsbfzslns.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gddssgffa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/ghjtzzpwr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gxngdvkkz.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gyrtcomfc.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gnweqaqrr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gelzfhyan.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gxxllflyy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gvffhrtjx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gwykwqnhz.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gmnephuha.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gofzznqzc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gtrdrubyt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/grthqvouh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/grzgxrzgy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqyizgbz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gcqdzhtlb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gwteoudqq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gqdbltxpj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/grgodbbrj.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gewlxzrxf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gheuxpkrb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gtwoxietr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/giijhljuh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/ghykpgguk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gcetrmujl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gnwsvgozl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/guyasenod.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gvcbaaqnb.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gtcebizik.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gmymjdsfo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gmvdibbgc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gkcrsnwbd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gorkzkjge.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/ggpuibobf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gmqcionor.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gtynwhvjn.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gedxpohbg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/guwoeyziq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gzcalsbws.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gupymklog.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gzkcyzxpz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gyitdrckj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gkkzaulms.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gnxftprin.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gsneaiqyl.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gswtnpmet.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gaozvziau.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gftowtwdt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gnxpaydum.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gkwyzmwss.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gnydnncoc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gjytqpwhi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gwdrdzjsw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gzwnsgbpf.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gqpwpmjrp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gutobuyfi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gegxydmvm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gjmricrau.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gtkqqgrnj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gtgkidenw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gfxacxsmb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/grsysdahe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gntqhaaqv.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/glryxqzmb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gwypeglkm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gqvinrwwr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gthupimuq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gopltjzla.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyiomuqsx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gfbcgnbhl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gewbulogn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/govisqdkk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpatzstew.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/ggzrqvfdn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaofazktr.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gvogoyrph.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gachcbboc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gqxzorbmc.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gqdvavfba.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guxrswsyu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gtpldqyqd.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gpomrwsdb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gltmekqdy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gjbniyjbd.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gmpjyaikz.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gcukbnolc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/glndbjvpd.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gkowtwjgy.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gjmxoketf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gsymianck.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/guportfxr.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gwtclbrdg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gmcdmfhwp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gtpdtaeri.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gwnkigvbn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gqbevqtaw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gwxbvntvp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gyitpqnof.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxabwjpsp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gaucudkre.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gqiggeadb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gqaqwadhp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gbufwcyxq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gbrboapre.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gfhftllma.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/grcgjtgzi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gdkokwamp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gcqmhdalt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gszvdfrkm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkjkxyvtg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/glhhouzem.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gcabgdppp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtcvqqfyq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gfqctkxqy.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gxxkyfwlf.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/ghfqibmry.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/guczyicfs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gasfvbsao.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gbsxyyvuf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/geeozidyc.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gqbmvzkio.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/guqjgyhvl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/grinobkau.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gnviiakfn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gnpfedkrf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gaakrqngl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gnjmjxppr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gtokvcdpq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gjjrutjar.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gvguqffyu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gkjaoiiao.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gaobbktpw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtlnqgber.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gduturfnc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gitujtcmf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gnqgzkkuu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gjiiobooz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gjidrupak.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gooiitidh.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gvrrrlaxp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gpibgkrlu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/ghqtnxbwq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gctslprty.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gdjzkxlez.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gusqhejkg.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gdpwqobwy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gmevezbos.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbkzufiit.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gmruniuli.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gilvtwvgx.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gafrnqreb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gzrlpyvll.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/ggdezkeju.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gpruwaozo.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gdnmhkywo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gkzsfclxd.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gofnypshm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gjvygaluv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gvtwnusyg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ghkhcvfki.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gxgdgfwyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/guqttuadf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gteyakqnu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gspntmwcr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gcxcoviud.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/glcwgpgis.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gdehafnxl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gbwplshzt.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/ggfehqlge.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gsasijsdw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gphugugrq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gxzdjiqvi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gfuirkknp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gsmydoytt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gxtuereck.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/grhfpxmfw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/giyhwqjck.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gxoagsiyc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gxdosfzll.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gpyvqtbih.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gpkfsazym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/grdgvhvbz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/ggbseexai.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/glaudxifl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gnmusfyjs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gcarsybgv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gewmasyvb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gsxdahqvo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gykiousno.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/glmgpztnd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gmitnuxvy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gmgpwfgar.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gnsdqinvm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gdtalilny.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gonftdyfs.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gvwgkelmh.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gjhsjppmr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gwvwocdol.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gcgdbaiac.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gcplvofzb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gdqvymwks.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gfxeonkse.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gwpwtkkww.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gmkufvobx.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gufigsgyr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gpeooqjnz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/guigbihca.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gftibconf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gyxpkiuzx.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gloxxpzlj.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gxwchubin.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gktvctknh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gzzinvmww.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/girkkstcy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gnanjhybn.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gykdxnwyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/glrcujnuh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gzdhhnlch.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gzipehxen.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gfuowozdu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gqtofixsp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gpookdbkb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glvfxlnbw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gvzlkylbv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjlzdyokv.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/grrislhmg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/ghvaqebeu.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gplwyaran.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/guqeltwda.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gkkalsmxy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gqzxmcffj.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gqagmcvlj.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gmxuarwaf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gvjmkirsu.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/giujryxvk.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gczdobdrg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmlayhyx.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gyzyclcob.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/goxzqhesb.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gukjhkoqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gguipceww.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gashqjrvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gfjcjjttd.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gmauhdrad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gslrgbmli.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/ggnfnwwdk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gcfpazroz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gpkejpxhc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gzkshfxix.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gjeostufd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gqgvceydg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gdphniymv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gdnnsiydh.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gjrgvhlsa.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gniplbckg.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gbcbgbdqf.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gqznovleo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gboxacjqw.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gbghlsdyv.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/giwclxusc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gwwoccyzk.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gstyuzhmd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbttrfztt.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gdobpnbkr.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdhelrkhj.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ggcboobvs.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gaytkzdlz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggjcxmzoe.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/ghiqtwvuf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gawqfmhbx.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/ghmrffbkv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gxddiwelo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/guutejmkm.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gyemvidrm.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gvtwysbvr.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/ghtyukrtv.sHtML


<!-- 参考信息 -->