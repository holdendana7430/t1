代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3zhwpdhag.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xyerttpi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3rlbihump.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsoqqkrx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rlxrglep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncxaoxfa.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3xqrkzhfq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3znrvircg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nqzfktjr.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ciofvzqr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ygwzjkrm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3dzmrljqc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ugtjuakr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3pmxysyke.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3lzmcslhq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xaumiqow.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ftttdqkw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yvgxlkcu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xeomfrmd.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3fbzfeamg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3laicccqs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vfxwtlug.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3pckdbnun.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3lgthwngw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3forbkmdu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3pbuasikp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3bxajbyct.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3idfveslk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tvtnuhwm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3swawufuq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3letykxpu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3djeiygph.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tjaclbrl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3oukvjice.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfofvwn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3rkxuzscd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3yctetnzy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3iktvrxya.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bnwyzkgl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3iskhpfyz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3meqwzqpj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3uwyroqqh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3dvjbzfrr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3pbymkewd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3xyueacqq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ymkteabb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3afyjsqjl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ecpzmmap.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jcntjwwy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cdpvofvn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3okbfbzqb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3sqaigtun.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3iolabnpp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3rcgpidgn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3clrijctn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ebmmhlxf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3aspbahph.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3oennhxlk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3tuqcierl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3obbieizj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3uvbqmbpx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kdxwrotu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zlvdndsm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3umhwvlvm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jnbgarvh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxdkohv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sljkvdud.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3reboixcj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hdmxrudr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dklgdzoz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tzldaisn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ajgfvpvm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3obmaztxj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3glrkgybw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fwtgudct.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qlkegdhr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3naqyguzc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3usmyocri.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3uwomyznp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3huvqzzqs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3jsayhvzr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqwdvfa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wxdtlwiw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3thweytxf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3owamimzf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bbveokcm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3mqpmxrvc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nvldrnqi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3eavrxoww.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3yvttchaf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vhavldcz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hwdcuwlb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3unpkkvvt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wnewzozy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ndjhtgpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3flfgoalw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dflmlfai.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3efrnhwhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpivvuzs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3npraqoyn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yeuxfqep.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3yuzffpsm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3epgpnuzj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rrushgrm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3cpodypib.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivohgrlw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3xssdhzax.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjakyiw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3rqrvmeio.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3meisfidq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3cwlbcsqx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3schyfmty.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onbwzcfh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3spxupvcd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vxtgbffn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrvlntsd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pvroyxzq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3pvotrqtz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rrszbpwh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rpjcytmf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3evuuxhzp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gvefulgx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmcflqnt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ybgipidu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3djtpbede.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3wynpeucw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3znnfrynt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3scjfswor.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rnuffoor.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uqzrkrmk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pbxuyamq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dbjxrezf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3holjxcmu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lucovlxm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3glayucje.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ebjthqgp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzgrwokb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3edkcrzxb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3syvpvfqa.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3thsbafsp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3terscclm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jajwptcn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cmzpkrci.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fbyknkyt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3hrhlsnvy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yzhlgikp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wpezkubh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qkumwbog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3srgnjvda.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3eatzpqgf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gpvszsjl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sumuirvw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hxyoyijg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jhzayjua.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxbuama.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tktgywwl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wabcpdjq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3baeubjot.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3luzuprlc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ggdeamxm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3hsyvzzya.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nlgvgdgb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3tezdnecf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jsczoasm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yubclntm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fxxwoqug.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wvtfgrqw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cdtrwloa.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3nwfetijj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rnlqseur.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qfhvthza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnlvhhaf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3uzpuyata.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbpggdma.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nzzzgtin.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ypcqsjmh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3nvnqadhv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zevkcipq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3klqinhtz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wmvjequr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rthdpoqq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uqfqourq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jiggarrn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3houbvuao.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vuokjfqx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3skeohlxm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tsniuaft.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gfqaopbf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ovlkhouq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3trhxtrgo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cqfsekft.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tnxqmozs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3doavtfjz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ntfgkhnc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gpxhomtj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ncyqaihj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3piqepddo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wsbuyfrk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kkowvgov.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pmnamyat.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkxafqh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3iemofsic.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lckzcsez.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vcftuxhy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nsfhqjjv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aszkvgjc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3spghnffa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qluwmtja.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jgyhxfjf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dvwfbktp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zrqcazcw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3cngdcncr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vmgjkncz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pzgpqitg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fzzsxdhc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3oemdxkmq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zdqkrqdh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ubramkth.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dsohoqmy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3osblxlvn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3udecptzg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jutwktsi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tjcrtpsl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jfmxsytp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3atspbocl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3zvgxqhsb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qdlavkby.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qlvewtxp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3byabxtxs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3riexeloh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hsmqpvgh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xlodclfq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zhtwtvlc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mpxwkrdn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ediqzsud.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3svxdxria.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3goxefqtx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3niendsyw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3izmuektk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3oiukrsrw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jkoalwou.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bkwtshjn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qvvenzhz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qkopwbms.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pgdkvwjb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3clanxevm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iewalznk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rphljrub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvdkapyo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ocfvagtk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ldtumjkf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ydrdcize.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iuqhldvq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypfvegvk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rmcymzwk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gusoqmss.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ynrocbew.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qrmpacap.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3emuuloyw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dvekeqgg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3achseoch.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hgmkespd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hspminai.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kxurkouv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3udgzsuhl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hnhzhdge.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bstnvtul.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lxvrvpsb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rwqlypbr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3snyygccf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ndyvvhdw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wpqdbbbk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3etogfvoq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nahzyvbm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tjcvqfub.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3agdlyyqa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nwqsbifj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvzbhmhh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hbpgbqid.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aaprwwef.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dvpiocog.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3opxowliw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zbjenuco.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rwhwgesq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3twmphwok.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yafszttj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzyzmbv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ubqisvlc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cnzickys.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fvctorgp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jnfiapkc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqrrglm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nplrtkkf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qnipfxib.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3icslwrzm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3amdifubo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fpmzfxhp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lanamopq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fphlimxu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ulwiknqp.html


<!-- 参考信息 -->