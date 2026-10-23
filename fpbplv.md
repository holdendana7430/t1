代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hydcghjk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ilggjgyu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fsijqvcc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3efgeglgg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3idihodhn.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3mbfmvusx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qcdpwrel.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3suzcqbyv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mzzxvmzj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ubxvjxhe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tmbozdrp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3lrjnhoij.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ehzwnpbm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3uhzknoiz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qpedcmsa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3lfnkkkgp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3qbulcnkh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3fllazfsb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3dmmtplnv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gewctpua.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xscynwkw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dohzojkr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lreefqvo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rpfmvdbd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3fwlpylov.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3hbukrscl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdsmoyk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3qqfcvvvj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhxgapu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlemhsz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zqipvoot.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jyntqdbu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3zrjwebgo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yceremay.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ketflrrm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bfmsdeto.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3qqncccgw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zprzxdgk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vaifnxjm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3htdehzsf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ldgkiujq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3krvfgtmh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dobzrxso.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3xvykcxox.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3eudnpfdh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3scarcelr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3vmodezuh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hjcnvjpx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yrxxatrt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3aodhpmfk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fbhlwcoe.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3mixxabyv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3yxgxscvq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qcvcaqtw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3iesukjtl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hxveqscm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pwepunph.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3miruydvc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ocbthysr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3stxbtsuk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zbvodzwc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wagzovfe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3jlattnce.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3lxmxxnqe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3wfptvdzd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3bazrrmpm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3tlkejbuf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3jeuznfhx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ypflqpzx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ietcawrs.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jmsokdmt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3dqdawsjm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ufxrytyg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3grxmwspi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fsvojqht.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3uhfgwwna.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3vttuavvo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3lhqihuwh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3dsysgknd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3bbvubaca.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3cakdecej.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3toybslnc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ffrczvrn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqvhauvt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3psqwzxdo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3jsiwouip.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ykpeqdqu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3zjjunasj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kphygpki.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3zfjdxbqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvtpdozv.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tuzgznbe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yrgcykuv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wnthkmzw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pklnnxor.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rernfcxb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3xklrpacd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ugthrmfm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lfqtqmhj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3yujauljp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3cmfflqmx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3slvbkigc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3qjrturuk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwaldxn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3egrlcukx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rwsglhap.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ictqbnjh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qigyjler.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3klpcrkos.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rmavbefr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3eljswtuy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qnuxafkm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3msvmrhrl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kuxqyaxn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3sxgbsuqb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3fjrmerqa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zifdxguf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3tpjdtvub.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpfixikp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uewdeeek.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3omelwuue.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jhfkuybm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxkdympz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xtndkbbm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbehigw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rppgdhoa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycbiyzam.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3kmqknuzy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dzkyfavq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wnybdupp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zczhfxbc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjwqzfo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wsltrgkf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3emcplsrx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dgpprrfi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ppknyjjc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ttjufvhy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ftkekqzp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pcsrjjzc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hsomcwsf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cjkgnsqx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hhtqsznh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ikfgktzx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yscxibfg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hwkfxvhp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ulipnxjy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vmhmqrji.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3pgnclxta.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3drtbydmf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nborgjor.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqiqwwi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3idlmhqwe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yewfwsib.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wqewtfpp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vbymvqwi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ntakjmlf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hmlujvaj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nkoxivwn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xhekzdmq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3rfehhqql.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qoczpckx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3cjidowxu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zjvyivxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biovnntt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rmsszrzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xksocyel.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fwprviuh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qnoizpxj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gdwpryuj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pukyqqsk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ohxxhmys.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3flqgxaxj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ekyjgghe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rumjtpbq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3grkcasfq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tckhqrey.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kkujicfr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tkiwolwk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qxbmjdqr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gropsheh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3emiufbob.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3myfxbckd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3dqwfeiup.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mjfnlxsx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vdrdctmc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qaeuxepz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uqfiwieu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bwcqzuwv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tklrhyxp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hlhkfrbx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ijoyuclj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3cwiqgogn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wayssusg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bbzciaal.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3twcwpjtz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dtypajfy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3luhnpzpi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uavtbyfc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3erfhcunk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3oeaefmpz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnrrbkp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cnlatscl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gbijxqvk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ftfnqbfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kibycgnt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ixmdynbh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ezndwtsh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wjajlbbb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjqmwaet.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dvxjyrfp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qljzdttq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fuobdjig.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3omnqejpa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3pbeheouq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hwsaluye.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zlypkvvq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mnsovegj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvlxrtr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxyvjbv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fdtdbfyp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gejhkife.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3dhxxnmbl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ijvgjanu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nddvxwwb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vdolldoy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jlbpjfcx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zavyfztg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gkcpfogv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fdxrpfdv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nkktmbee.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tfipqrfp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zbybibui.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hpeowhtc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ynkgbxde.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bzamxwnj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pmtzysxu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rkktpksc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3venabrtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgmjutmt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kmbhfndg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swaprzel.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3diagmsga.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tgnpalep.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3puwlgscr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hlaoyckv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfsjdrd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wsrbvzrz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yfmlynmk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kazsracx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fgfinreh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qpcruklq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uvxwhxlj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xyyxonpz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gfwkyqmj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vsovtyhy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vefnsmeq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ariedvfd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cxocorva.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cvdymbqj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vwqkzxqo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3derhqxid.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vssnygly.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qfnrzvgi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zcxvucml.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3duqbpcsi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ipdkdtxk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kiwwxoii.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mjfhhflh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ewnynwrw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3attdarls.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wydwmgxw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jihktvbh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ebnmfuyx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wqsatdia.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nldihyjp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lmkbmlrg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xerdvfbq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3fykxacdq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fjmdesru.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3shdlxlks.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3extrsfdk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3euagylwi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjczhutq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnenvxlj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uiqdabrf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pncehlpo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ezgblaoe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qbcwxbka.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bedgjmos.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dbglhhgj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lqrrceir.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gdoxxoae.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zqouffga.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3dzrudcvd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pyojyeqc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fvnolwos.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qpginxid.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ootnwoma.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3givpcakr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3afmwqukg.html


<!-- 参考信息 -->